# Comparing `tmp/dbt_copilot_tools-0.1.2.tar.gz` & `tmp/dbt_copilot_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_copilot_tools-0.1.2.tar", max compression
+gzip compressed data, was "dbt_copilot_tools-0.1.3.tar", max compression
```

## Comparing `dbt_copilot_tools-0.1.2.tar` & `dbt_copilot_tools-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.2/LICENSE
--rw-r--r--   0        0        0     1209 2023-06-16 14:14:21.704068 dbt_copilot_tools-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.2/commands/__init__.py
--rwxr-xr-x   0        0        0     9980 2023-06-14 12:11:53.497780 dbt_copilot_tools-0.1.2/commands/bootstrap_cli.py
--rwxr-xr-x   0        0        0    11242 2023-06-15 11:49:38.161070 dbt_copilot_tools-0.1.2/commands/codebuild_cli.py
--rwxr-xr-x   0        0        0     8582 2023-06-15 16:41:34.056908 dbt_copilot_tools-0.1.2/commands/copilot_cli.py
--rwxr-xr-x   0        0        0    20700 2023-06-19 10:28:42.526261 dbt_copilot_tools-0.1.2/commands/dns_cli.py
--rw-r--r--   0        0        0     5902 2023-06-16 11:05:25.989196 dbt_copilot_tools-0.1.2/commands/utils.py
--rwxr-xr-x   0        0        0      656 2023-06-16 11:24:09.621662 dbt_copilot_tools-0.1.2/copilot_helper.py
--rw-r--r--   0        0        0     1139 2023-06-19 14:04:34.232750 dbt_copilot_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1593 2023-06-21 10:28:30.704825 dbt_copilot_tools-0.1.3/commands/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.3/commands/__init__.py
+-rwxr-xr-x   0        0        0     9980 2023-06-21 10:25:13.933813 dbt_copilot_tools-0.1.3/commands/bootstrap_cli.py
+-rwxr-xr-x   0        0        0     2560 2023-06-20 14:07:55.205282 dbt_copilot_tools-0.1.3/commands/check_cloudformation.py
+-rwxr-xr-x   0        0        0    13488 2023-06-20 09:47:08.337250 dbt_copilot_tools-0.1.3/commands/codebuild_cli.py
+-rwxr-xr-x   0        0        0     8582 2023-06-15 16:41:34.056908 dbt_copilot_tools-0.1.3/commands/copilot_cli.py
+-rwxr-xr-x   0        0        0    20699 2023-06-20 09:47:08.337507 dbt_copilot_tools-0.1.3/commands/dns_cli.py
+-rw-r--r--   0        0        0     5902 2023-06-16 11:05:25.989196 dbt_copilot_tools-0.1.3/commands/utils.py
+-rwxr-xr-x   0        0        0      803 2023-06-20 14:07:55.205587 dbt_copilot_tools-0.1.3/copilot_helper.py
+-rw-r--r--   0        0        0     1169 2023-06-21 10:25:23.727055 dbt_copilot_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.3/PKG-INFO
```

### Comparing `dbt_copilot_tools-0.1.2/LICENSE` & `dbt_copilot_tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.2/commands/bootstrap_cli.py` & `dbt_copilot_tools-0.1.3/commands/bootstrap_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.2/commands/codebuild_cli.py` & `dbt_copilot_tools-0.1.3/commands/codebuild_cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 
 def check_github_conn(client: CodeBuildClient):
     response = client.list_source_credentials()
 
     # If there are no source code creds defined then AWS is not linked to Github
     if not response["sourceCredentialsInfos"]:
-        if not click.confirm(click.style("GitHub is not linked in this AWS account\nDo you want to link with a PAT?", fg="yellow")):
+        if not click.confirm(click.style(
+                "GitHub is not linked in this AWS account\nDo you want to link with a PAT?", fg="yellow")):
             exit()
 
         pat = input(
             """
             Create a bots PAT with the following scope:
                 repo:   status: Grants read/write access to public and private repository commit statuses.
                 admin:  repo_hook: Grants full control of repository hooks.
@@ -40,23 +41,27 @@
             Enter in the PAT here:
             """,
         )
 
         import_pat(pat, client)
 
 
-def check_service_role(project_session: Session) -> str:
+def check_service_role(role_name, project_session: Session) -> str:
     client = project_session.client("iam", region_name=AWS_REGION)
 
     try:
-        response = client.get_role(RoleName="ci-CodeBuild-role")
+        response = client.get_role(RoleName=role_name)
         role_arn = response["Role"]["Arn"]
 
     except client.exceptions.NoSuchEntityException:
-        click.secho("Role for service does not exist; run ./codebuild_cli.py create-codeploy-role", fg="cyan")
+        click.echo(
+            click.style("Service Role", fg="yellow") +
+            click.style(f" {role_name} ", fg="white", bold=True) +
+            click.style("does not exist; run: ", fg="yellow") +
+            click.style("copilot-helper.py codebuild create-codedeploy-role --type <ci/custom>", fg="cyan"))
         role_arn = ""
         exit()
 
     return role_arn
 
 
 def update_parameter(project_session: Session, name: str, description: str, value: str):
@@ -87,117 +92,28 @@
             click.style("Unable to recognise Git URL format, make sure it is either:\n", fg="red") +
             click.style("https://github.com/<org>/<repository-name>\n" +
             "git@github.com:<org>/<repository-name>", fg="white", bold=True))
         exit()
     return git_url
 
 
-@click.group()
-def codebuild():
-    pass
-
-
-@codebuild.command()
-@click.option("--pat", help="PAT Token", required=True)
-@click.option("--project-profile", help="aws account profile name", required=True)
-def link_github(pat: str, project_profile: str) -> None:
-    """Links CodeDeploy to Github via users PAT."""
-    project_session = check_aws_conn(project_profile)
-    client = project_session.client("codebuild", region_name=AWS_REGION)
-    import_pat(pat, client)
-
-
-@codebuild.command()
-@click.option("--project-profile", help="aws account profile name", required=True)
-def create_codedeploy_role(project_profile: str) -> None:
-    """Add AWS Role needed for codedeploy."""
-
-    project_session = check_aws_conn(project_profile)
-    account_id = project_session.client("sts").get_caller_identity().get("Account")
-
-    current_filepath = os.path.dirname(os.path.realpath(__file__))
-
-    with open(f"{current_filepath}/../templates/put-codebuild-role-policy.json") as f:
-        policy_doc = json.load(f)
-    client = project_session.client("iam", region_name=AWS_REGION)
-
-    # A policy must be defined if not present.
-    try:
-        response = client.create_policy(
-            PolicyName="ci-CodeBuild-policy",
-            PolicyDocument=json.dumps(policy_doc),
-            Description="Custom Policy for codebuild",
-            Tags=[
-                {"Key": "Name", "Value": "CustomPolicy"},
-            ],
-        )
-        check_response(response)
-        click.secho("Policy created", fg="green")
-
-    except client.exceptions.EntityAlreadyExistsException:
-        if not click.confirm(click.style("Policy exists.\nDo you want to update it?", fg="yellow")):
-            exit()
-        try:
-            response = client.create_policy_version(
-                PolicyArn=f"arn:aws:iam::{account_id}:policy/ci-CodeBuild-policy",
-                PolicyDocument=json.dumps(policy_doc),
-                SetAsDefault=True,
-            )
-            check_response(response)
-            click.secho("Policy updated", fg="green")
-
-        except client.exceptions.LimitExceededException:
-            click.secho("You have hit the limit of max managed policies, please delete an existing version and try again", fg="red")
-            exit()
-
-    with open(f"{current_filepath}/../templates/create-codebuild-role.json") as f:
-        role_doc = json.load(f)
-
-    # Now create a role if not present and attache policy
-    try:
-        response = client.create_role(RoleName="ci-CodeBuild-role", AssumeRolePolicyDocument=json.dumps(role_doc))
-        check_response(response)
-        click.secho("Role created", fg="green")
-    except client.exceptions.EntityAlreadyExistsException:
-        click.secho("Role exists", fg="yellow")
-
-    response = client.attach_role_policy(
-        PolicyArn=f"arn:aws:iam::{account_id}:policy/ci-CodeBuild-policy",
-        RoleName="ci-CodeBuild-role",
-    )
-    check_response(response)
-    click.secho("Policy attached to Role", fg="green")
-
-
-@codebuild.command()
-@click.option("--update", is_flag=True, show_default=True, default=False, help="Update config")
-@click.option("--name", required=True, help="Name of project")
-@click.option("--desc", default="", help="Description of project")
-@click.option("--git", required=True, help="Git url of code")
-@click.option("--branch", required=True, help="Git branch")
-@click.option("--buildspec", required=True, help="Location of buildspec file in repo")
-@click.option("--builderimage", default=DEFAULT_CI_BUILDER, help="Builder image")
-@click.option("--project-profile", required=True, help="aws account profile name")
-@click.option("--release", is_flag=True, show_default=True, default=False, help="Trigger builds on release tags")
-def codedeploy(update, name, desc, git, branch, buildspec, builderimage, project_profile, release):
-    """Builds Code build boilerplate."""
+def modify_project(project_session, update, name, desc, git, branch, buildspec, builderimage, release, role_type):
 
     git_url = check_git_url(git)
-    project_session = check_aws_conn(project_profile)
-    role_arn = check_service_role(project_session)
+    role_arn = check_service_role("ci-CodeBuild-role", project_session)
     client = project_session.client("codebuild", region_name=AWS_REGION)
     check_github_conn(client)
 
     environment = {
         "type": "LINUX_CONTAINER",
         "image": f"{builderimage}",
         "computeType": "BUILD_GENERAL1_SMALL",
         "environmentVariables": [],
         "privilegedMode": True,
-        "imagePullCredentialsType": "SERVICE_ROLE",
+        "imagePullCredentialsType": f"{role_type}",
     }
 
     source = {
         "type": "GITHUB",
         "location": f"{git_url}",
         "buildspec": f"{buildspec}",
         "auth": {"type": "OAUTH", "resource": "AWS::CodeBuild::SourceCredential"},
@@ -242,15 +158,14 @@
                         "pattern": "PUSH",
                     },
                     {"type": "HEAD_REF", "pattern": pattern},
                 ],
             ],
             buildType="BUILD",
         )
-        click.secho("Project Updated", fg="green")
 
     else:
         try:
             response = client.create_project(
                 name=name,
                 description=desc,
                 source=source,
@@ -277,17 +192,148 @@
 
         except client.exceptions.ResourceAlreadyExistsException:
             click.secho("Project already exists, use the --update flag", fg="red")
             exit()
 
     check_response(response)
     check_response(response_webhook)
-    click.echo(click.style("Codebuild project", fg="yellow") +
-                           click.style(f"{name}",fg="white", bold=True) +
-                           click.style("created", fg="yellow"))
+    click.echo(click.style("Codebuild project ", fg="yellow") +
+                click.style(f"{name} ",fg="white", bold=True) +
+                click.style("updated", fg="yellow"))
+
+
+@click.group()
+def codebuild():
+    pass
+
+
+@codebuild.command()
+@click.option("--pat", help="PAT Token", required=True)
+@click.option("--project-profile", help="aws account profile name", required=True)
+def link_github(pat: str, project_profile: str) -> None:
+    """Links CodeDeploy to Github via users PAT."""
+    project_session = check_aws_conn(project_profile)
+    client = project_session.client("codebuild", region_name=AWS_REGION)
+    import_pat(pat, client)
+
+
+@codebuild.command()
+@click.option("--project-profile", help="aws account profile name", required=True)
+@click.option("--type", type=click.Choice(["ci", "custom"]), help="type of project <ci/custom>", default="ci")
+def create_codedeploy_role(project_profile: str, type) -> None:
+    """Add AWS Role needed for codedeploy."""
+
+    project_session = check_aws_conn(project_profile)
+    account_id = project_session.client("sts").get_caller_identity().get("Account")
+
+    current_filepath = os.path.dirname(os.path.realpath(__file__))
+
+    with open(f"{current_filepath}/../templates/{type}-codebuild-role-policy.json") as f:
+        policy_doc = json.load(f)
+    client = project_session.client("iam", region_name=AWS_REGION)
+
+    # A policy must be defined if not present.
+    try:
+        response = client.create_policy(
+            PolicyName=f"{type}-CodeBuild-policy",
+            PolicyDocument=json.dumps(policy_doc),
+            Description="Custom Policy for codebuild",
+            Tags=[
+                {"Key": "Name", "Value": "CustomPolicy"},
+            ],
+        )
+        check_response(response)
+        click.secho("Policy created", fg="green")
+
+    except client.exceptions.EntityAlreadyExistsException:
+        if not click.confirm(click.style("Policy exists.\nDo you want to update it?", fg="yellow")):
+            exit()
+        try:
+            response = client.create_policy_version(
+                PolicyArn=f"arn:aws:iam::{account_id}:policy/{type}-CodeBuild-policy",
+                PolicyDocument=json.dumps(policy_doc),
+                SetAsDefault=True,
+            )
+            check_response(response)
+            click.secho("Policy updated", fg="green")
+
+        except client.exceptions.LimitExceededException:
+            click.secho(
+                "You have hit the limit of max managed policies, "
+                "please delete an existing version and try again", fg="red")
+            exit()
+
+    with open(f"{current_filepath}/../templates/create-codebuild-role.json") as f:
+        role_doc = json.load(f)
+
+    # Now create a role if not present and attach policy
+    try:
+        response = client.create_role(RoleName=f"{type}-CodeBuild-role", AssumeRolePolicyDocument=json.dumps(role_doc))
+        check_response(response)
+        click.secho("Role created", fg="green")
+    except client.exceptions.EntityAlreadyExistsException:
+        click.secho("Role exists", fg="yellow")
+
+    response = client.attach_role_policy(
+        PolicyArn=f"arn:aws:iam::{account_id}:policy/{type}-CodeBuild-policy",
+        RoleName=f"{type}-CodeBuild-role",
+    )
+    check_response(response)
+    click.secho("Policy attached to Role", fg="green")
+
+
+@codebuild.command()
+@click.option("--update", is_flag=True, show_default=True, default=False, help="Update config")
+@click.option("--name", required=True, help="Name of project")
+@click.option("--desc", default="", help="Description of project")
+@click.option("--git", required=True, help="Git url of code")
+@click.option("--branch", required=True, help="Git branch")
+@click.option("--buildspec", required=True, help="Location of buildspec file in repo")
+@click.option("--builderimage", default=DEFAULT_CI_BUILDER, help="Builder image")
+@click.option("--project-profile", required=True, help="aws account profile name")
+@click.option("--release", is_flag=True, show_default=True, default=False, help="Trigger builds on release tags")
+def codedeploy(update, name, desc, git, branch, buildspec, builderimage, project_profile, release):
+    """Builds Code build boilerplate."""
+
+    project_session = check_aws_conn(project_profile)
+    modify_project(project_session, update, name, desc, git, branch, buildspec, builderimage, release, "SERVICE_ROLE")
+
+
+@codebuild.command()
+@click.option("--update", is_flag=True, show_default=True, default=False, help="Update config")
+@click.option("--name", required=True, help="Name of project")
+@click.option("--desc", default="", help="Description of project")
+@click.option("--git", required=True, help="Git url of code")
+@click.option("--branch", required=True, help="Git branch")
+@click.option("--buildspec", required=True, help="Location of buildspec file in repo")
+@click.option("--builderimage", default="aws/codebuild/amazonlinux2-x86_64-standard:3.0", help="Builder image")
+@click.option("--project-profile", required=True, help="aws account profile name")
+def buildproject(update, name, desc, git, branch, buildspec, builderimage, project_profile):
+    """Builds Code build for ad hoc projects."""
+
+    project_session = check_aws_conn(project_profile)
+    modify_project(project_session, update, name, desc, git, branch, buildspec, builderimage, False, "CODEBUILD")
+
+
+@codebuild.command()
+@click.option("--name", required=True, help="Name of project")
+@click.option("--project-profile", required=True, help="aws account profile name")
+def delete_project(name, project_profile):
+    """Delete CodeBuild projects."""
+
+    project_session = check_aws_conn(project_profile)
+    client = project_session.client("codebuild", region_name=AWS_REGION)
+
+    if not click.confirm(click.style("Are you sure you want to delete the project ", fg="yellow") +
+                         click.style(f"{name}", fg="white", bold=True)):
+        exit()
+
+    response = client.delete_project(name=name)
+    check_response(response)
+    click.secho("Project deleted", fg="green")
 
 
 @codebuild.command()
 @click.option("--workspace", help="Slack Workspace id", required=True)
 @click.option("--channel", help="Slack channel id", required=True)
 @click.option("--token", help="Slack api token", required=True)
 @click.option("--project-profile", help="aws account profile name", required=True)
@@ -302,15 +348,15 @@
             "value": workspace,
         },
         "channel": {"name": "/codebuild/slack_channel_id", "description": "Slack Channel ID", "value": channel},
         "token": {"name": "/codebuild/slack_api_token", "description": "Slack API Token", "value": token},
     }
 
     if not click.confirm(click.style(
-        "Updating Parameter Store with Slack credentials.\nDo you want to update it?", fg="yellow")):
+            "Updating Parameter Store with Slack credentials.\nDo you want to update it?", fg="yellow")):
         exit()
 
     for item, value in SLACK.items():
         update_parameter(project_session, value["name"], value["description"], value["value"])
     click.secho("Paramater Store updated", fg="green")
```

### Comparing `dbt_copilot_tools-0.1.2/commands/copilot_cli.py` & `dbt_copilot_tools-0.1.3/commands/copilot_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.2/commands/dns_cli.py` & `dbt_copilot_tools-0.1.3/commands/dns_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,18 +173,18 @@
                     },
                 ],
             },
         )
 
     check_response(response)
     click.echo(
-        click.style(f"{records['Name']}, Type: {records['Type']}", fg="white", bold=True)
-        + click.style("Added.", fg="magenta"),
-    )
-    return response["ChangeInfo"]["Status"]
+        click.style(f"{records['Name']}, Type: {records['Type']}", fg="white", bold=True) +
+        click.style("Added.", fg="magenta")
+        )
+    return response['ChangeInfo']['Status']
 
 
 def check_for_records(client, parent_id, subdom, subdom_id):
     records_to_add = []
     response = client.list_resource_record_sets(
         HostedZoneId=parent_id,
     )
@@ -281,17 +281,16 @@
 
     # Check if base domain is valid
     if base_domain[-1] != ".":
         base_domain = base_domain + "."
 
     if base_domain not in hosted_zones:
         click.secho(
-            f"The base domain: {base_domain} does not exist in your AWS domain account {response['HostedZones']}",
-            fg="red",
-        )
+            f"The base domain: {base_domain} does not exist in your AWS domain account \
+                {response['HostedZones']}", fg='red')
         exit()
 
     base_len = len(base_domain.split(".")) - 1
     parts = domain.split(".")
 
     for _ in range(len(parts) - 1):
         subdom = ".".join(parts) + "."
```

### Comparing `dbt_copilot_tools-0.1.2/commands/utils.py` & `dbt_copilot_tools-0.1.3/commands/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.2/pyproject.toml` & `dbt_copilot_tools-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.black]
 line-length = 119
 
 [tool.poetry]
 name = "dbt-copilot-tools"
-version = "0.1.2"
+version = "0.1.3"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
-readme = "README.md"
+readme = "commands/README.md"
 packages = [
     { include = "commands" },
     { include = "copilot_helper.py" }
 ]
 
 [tool.poetry.scripts]
 copilot-helper = "copilot_helper:cli"
@@ -26,14 +26,15 @@
 cloudfoundry-client = "1.34.1"
 jsonschema = "4.17.3"
 mypy-boto3-codebuild = "1.26.0.post1"
 python = "^3.9"
 schema = "0.7.5"
 
 [tool.poetry.group.dev.dependencies]
+cfn-lint = "^0.77.7"
 moto = "^4.1.11"
 pyfakefs = "^5.2.2"
 pytest = "^7.3.1"
 pytest-env = "^0.8.1"
 tox = "^4.6.0"
 
 [tool.poetry.group.pre-commit]
```

