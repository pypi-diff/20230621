# Comparing `tmp/kubedeployer-1.2.2.tar.gz` & `tmp/kubedeployer-1.2.3.tar.gz`

## Comparing `kubedeployer-1.2.2.tar` & `kubedeployer-1.2.3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/.dockerignore
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/.pylintrc
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/Dockerfile
--rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeploy
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/pytest.ini
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/requirements.txt
--rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/docs/ru.md
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/__main__.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/deploy.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/docker.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/files.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/kubectl.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/kustomize.py
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/manifests.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/text.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/types.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/console/__init__.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/console/wrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/deployer/__init__.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/deployer/abstract_deployer.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/deployer/kustomize_deployer.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/deployer/orthodox_deployer.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/deployer/smart_deployer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/gitlab_ci/__init__.py
--rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/gitlab_ci/environment_variables.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/gitlab_ci/exceptions.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/gitlab_ci/specification.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/gitlab_ci/variable_reader.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/gitlab_ci/variable_types.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/k8s/__init__.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/k8s/annotations.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/k8s/deserialize.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/k8s/models.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/k8s/specifications.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/__init__.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/kubesec/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/kubesec/data.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/kubesec/errors.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/kubesec/formatters.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/kubesec/report.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/kubesec/scanner.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/trivy/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/trivy/data.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/trivy/errors.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/trivy/formatters.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/trivy/report.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/security/trivy/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/utils/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/utils/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/vault/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/vault/client.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/vault/factory.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/kubedeployer/vault/service.py
--rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/scripts/run_e2e_tests.sh
--rwxr-xr-x   0        0        0      429 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/scripts/run_tests.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/conftest.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/mocks.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/containers/Dockerfile
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/containers/docker-compose.yaml
--rwxr-xr-x   0        0        0      737 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/containers/entrypoint.sh
--rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/containers/e2e_tests/e2e_entrypoint.sh
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/containers/integration_tests/docker-compose.yaml
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/containers/integration_tests/integration_entrypoint.sh
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/containers/kind/config.yaml
--rwxr-xr-x   0        0        0      983 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/containers/kind/prepare-kind.sh
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/containers/manifests/rbac.yaml
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/envs/base
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/envs/override
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/env-manifest.yaml
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/manifests.yaml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/env-app/manifest.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/env-app/production/ingress.yaml
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app/base/deployment.yaml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app/base/kustomization.yaml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app/base/service.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app/overlays/stage/configmap.yaml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app/overlays/stage/kustomization.yaml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app-with-env/base/kustomization.yaml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app-with-env/base/service.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/configmap.yaml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/kustomization.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/non-kustomize-app/deployment.yaml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/non-kustomize-app/service.yaml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/non-kustomize-app/stage/configmap.yaml
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/non-kustomize-app-with-env/service.yaml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/data/manifests/apps/non-kustomize-app-with-env/stage/configmap.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/integration/__init__.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/integration/conftest.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/integration/test_args.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/integration/test_deployer.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/integration/test_k8s.py
--rw-r--r--   0        0        0    10161 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/integration/test_kubedeployer.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/integration/test_kustomize.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/integration/test_security_kubesec.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/integration/test_security_trivy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/integration/vault/__init__.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/integration/vault/mocks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/unit/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/unit/test_console.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/unit/test_console_wrap.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/unit/test_deployer.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/unit/test_files.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/unit/test_manifests.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/unit/test_text.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/unit/test_utils_convert.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/tests/unit/test_vault.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/LICENSE
--rw-r--r--   0        0        0     8852 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/README.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    22542 2020-02-02 00:00:00.000000 kubedeployer-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/.dockerignore
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/.pylintrc
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/Dockerfile
+-rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeploy
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/pytest.ini
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/requirements.txt
+-rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/docs/ru.md
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/__main__.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/deploy.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/docker.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/files.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/kubectl.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/kustomize.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/manifests.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/text.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/types.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/console/__init__.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/console/wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/deployer/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/deployer/abstract_deployer.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/deployer/kustomize_deployer.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/deployer/orthodox_deployer.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/deployer/smart_deployer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/gitlab_ci/__init__.py
+-rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/gitlab_ci/environment_variables.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/gitlab_ci/exceptions.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/gitlab_ci/specification.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/gitlab_ci/variable_reader.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/gitlab_ci/variable_types.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/k8s/__init__.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/k8s/annotations.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/k8s/deserialize.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/k8s/models.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/k8s/specifications.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/__init__.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/kubesec/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/kubesec/data.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/kubesec/errors.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/kubesec/formatters.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/kubesec/report.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/kubesec/scanner.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/trivy/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/trivy/data.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/trivy/errors.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/trivy/formatters.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/trivy/report.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/security/trivy/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/utils/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/utils/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/vault/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/vault/client.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/vault/factory.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/kubedeployer/vault/service.py
+-rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/scripts/run_e2e_tests.sh
+-rwxr-xr-x   0        0        0      429 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/scripts/run_tests.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/conftest.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/mocks.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/containers/Dockerfile
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/containers/docker-compose.yaml
+-rwxr-xr-x   0        0        0      737 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/containers/entrypoint.sh
+-rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/containers/e2e_tests/e2e_entrypoint.sh
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/containers/integration_tests/docker-compose.yaml
+-rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/containers/integration_tests/integration_entrypoint.sh
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/containers/kind/config.yaml
+-rwxr-xr-x   0        0        0      983 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/containers/kind/prepare-kind.sh
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/containers/manifests/rbac.yaml
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/envs/base
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/envs/override
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/env-manifest.yaml
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/manifests.yaml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/env-app/manifest.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/env-app/production/ingress.yaml
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app/base/deployment.yaml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app/base/kustomization.yaml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app/base/service.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app/overlays/stage/configmap.yaml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app/overlays/stage/kustomization.yaml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app-with-env/base/kustomization.yaml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app-with-env/base/service.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/configmap.yaml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/kustomization.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/non-kustomize-app/deployment.yaml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/non-kustomize-app/service.yaml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/non-kustomize-app/stage/configmap.yaml
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/non-kustomize-app-with-env/service.yaml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/data/manifests/apps/non-kustomize-app-with-env/stage/configmap.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/integration/__init__.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/integration/conftest.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/integration/test_args.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/integration/test_deployer.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/integration/test_k8s.py
+-rw-r--r--   0        0        0    10161 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/integration/test_kubedeployer.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/integration/test_kustomize.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/integration/test_security_kubesec.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/integration/test_security_trivy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/integration/vault/__init__.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/integration/vault/mocks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/unit/test_console.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/unit/test_console_wrap.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/unit/test_deployer.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/unit/test_files.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/unit/test_manifests.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/unit/test_text.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/unit/test_utils_convert.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/tests/unit/test_vault.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/LICENSE
+-rw-r--r--   0        0        0     9373 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/README.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    23063 2020-02-02 00:00:00.000000 kubedeployer-1.2.3/PKG-INFO
```

### Comparing `kubedeployer-1.2.2/.pylintrc` & `kubedeployer-1.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/Dockerfile` & `kubedeployer-1.2.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/.github/workflows/ci.yml` & `kubedeployer-1.2.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/docs/ru.md` & `kubedeployer-1.2.3/docs/ru.md`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/__init__.py` & `kubedeployer-1.2.3/kubedeployer/__init__.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/deploy.py` & `kubedeployer-1.2.3/kubedeployer/deploy.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/docker.py` & `kubedeployer-1.2.3/kubedeployer/docker.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/files.py` & `kubedeployer-1.2.3/kubedeployer/files.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/kubectl.py` & `kubedeployer-1.2.3/kubedeployer/kubectl.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/kustomize.py` & `kubedeployer-1.2.3/kubedeployer/kustomize.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/manifests.py` & `kubedeployer-1.2.3/kubedeployer/manifests.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/text.py` & `kubedeployer-1.2.3/kubedeployer/text.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/console/__init__.py` & `kubedeployer-1.2.3/kubedeployer/console/__init__.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/console/wrap.py` & `kubedeployer-1.2.3/kubedeployer/console/wrap.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/deployer/kustomize_deployer.py` & `kubedeployer-1.2.3/kubedeployer/deployer/kustomize_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/deployer/orthodox_deployer.py` & `kubedeployer-1.2.3/kubedeployer/deployer/orthodox_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/deployer/smart_deployer.py` & `kubedeployer-1.2.3/kubedeployer/deployer/smart_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/gitlab_ci/environment_variables.py` & `kubedeployer-1.2.3/kubedeployer/gitlab_ci/environment_variables.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/gitlab_ci/specification.py` & `kubedeployer-1.2.3/kubedeployer/gitlab_ci/specification.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/gitlab_ci/variable_reader.py` & `kubedeployer-1.2.3/kubedeployer/gitlab_ci/variable_reader.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/gitlab_ci/variable_types.py` & `kubedeployer-1.2.3/kubedeployer/gitlab_ci/variable_types.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/k8s/annotations.py` & `kubedeployer-1.2.3/kubedeployer/k8s/annotations.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/k8s/models.py` & `kubedeployer-1.2.3/kubedeployer/k8s/models.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/security/kubesec/data.py` & `kubedeployer-1.2.3/kubedeployer/security/kubesec/data.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/security/kubesec/formatters.py` & `kubedeployer-1.2.3/kubedeployer/security/kubesec/formatters.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/security/kubesec/report.py` & `kubedeployer-1.2.3/kubedeployer/security/kubesec/report.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/security/kubesec/scanner.py` & `kubedeployer-1.2.3/kubedeployer/security/kubesec/scanner.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/security/trivy/data.py` & `kubedeployer-1.2.3/kubedeployer/security/trivy/data.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/security/trivy/formatters.py` & `kubedeployer-1.2.3/kubedeployer/security/trivy/formatters.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/security/trivy/scanner.py` & `kubedeployer-1.2.3/kubedeployer/security/trivy/scanner.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/vault/client.py` & `kubedeployer-1.2.3/kubedeployer/vault/client.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/vault/factory.py` & `kubedeployer-1.2.3/kubedeployer/vault/factory.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/kubedeployer/vault/service.py` & `kubedeployer-1.2.3/kubedeployer/vault/service.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/scripts/run_e2e_tests.sh` & `kubedeployer-1.2.3/scripts/run_e2e_tests.sh`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/conftest.py` & `kubedeployer-1.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/mocks.py` & `kubedeployer-1.2.3/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/containers/Dockerfile` & `kubedeployer-1.2.3/tests/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/containers/entrypoint.sh` & `kubedeployer-1.2.3/tests/containers/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/containers/e2e_tests/e2e_entrypoint.sh` & `kubedeployer-1.2.3/tests/containers/e2e_tests/e2e_entrypoint.sh`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/containers/kind/config.yaml` & `kubedeployer-1.2.3/tests/containers/kind/config.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/containers/kind/prepare-kind.sh` & `kubedeployer-1.2.3/tests/containers/kind/prepare-kind.sh`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/containers/manifests/rbac.yaml` & `kubedeployer-1.2.3/tests/containers/manifests/rbac.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/data/manifests/env-manifest.yaml` & `kubedeployer-1.2.3/tests/data/manifests/env-manifest.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/data/manifests/manifests.yaml` & `kubedeployer-1.2.3/tests/data/manifests/manifests.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/data/manifests/apps/env-app/manifest.yaml` & `kubedeployer-1.2.3/tests/data/manifests/apps/env-app/manifest.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/data/manifests/apps/env-app/production/ingress.yaml` & `kubedeployer-1.2.3/tests/data/manifests/apps/env-app/production/ingress.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app/base/deployment.yaml` & `kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml` & `kubedeployer-1.2.3/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/data/manifests/apps/non-kustomize-app/deployment.yaml` & `kubedeployer-1.2.3/tests/data/manifests/apps/non-kustomize-app/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml` & `kubedeployer-1.2.3/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/integration/test_args.py` & `kubedeployer-1.2.3/tests/integration/test_args.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/integration/test_deployer.py` & `kubedeployer-1.2.3/tests/integration/test_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/integration/test_k8s.py` & `kubedeployer-1.2.3/tests/integration/test_k8s.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/integration/test_kubedeployer.py` & `kubedeployer-1.2.3/tests/integration/test_kubedeployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/integration/test_kustomize.py` & `kubedeployer-1.2.3/tests/integration/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/integration/test_security_kubesec.py` & `kubedeployer-1.2.3/tests/integration/test_security_kubesec.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/integration/test_security_trivy.py` & `kubedeployer-1.2.3/tests/integration/test_security_trivy.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/unit/test_console_wrap.py` & `kubedeployer-1.2.3/tests/unit/test_console_wrap.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/unit/test_deployer.py` & `kubedeployer-1.2.3/tests/unit/test_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/unit/test_files.py` & `kubedeployer-1.2.3/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/unit/test_manifests.py` & `kubedeployer-1.2.3/tests/unit/test_manifests.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/unit/test_text.py` & `kubedeployer-1.2.3/tests/unit/test_text.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/unit/test_utils_convert.py` & `kubedeployer-1.2.3/tests/unit/test_utils_convert.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/tests/unit/test_vault.py` & `kubedeployer-1.2.3/tests/unit/test_vault.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/.gitignore` & `kubedeployer-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/LICENSE` & `kubedeployer-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/README.md` & `kubedeployer-1.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,20 @@
 ### Options
 
 * __-d__, __-deployer__=smart: structure maintenance types
 (see Supported structure maintenance types);
 * __--dry-run__: only show built manifest without apply it;
 * __--env-file__ list: read in a file of environment variables. If environment
 variable does contain in several files, then it will be has value from last file.
+* __--project-dir \<path\>__: full path to folder with project, if it is not setted,
+used value from environment variable `CI_PROJECT_DIR`, if variable is not setted, as 
+default value used current working directory
+* __--environment \<env_name\>__: environment for builder, if it is not setted, used
+value from environment variable `ENVIRONMENT`
+* __--manifest-folder \<path\>__: path to folder with manifest, path is relative to project_dir. If it is not set, will get value from environment variable `MANIFEST_FOLDER`
 
 ## Supported structure maintenance types
 
 Kubedeployer supports three structure maintenance types of manifests to deploy:
 - orthodox
 - smart - this one is default
 - kustomize
```

### Comparing `kubedeployer-1.2.2/pyproject.toml` & `kubedeployer-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.2.2/PKG-INFO` & `kubedeployer-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubedeployer
-Version: 1.2.2
+Version: 1.2.3
 Summary: package to deploy application on kubernetes
 Project-URL: Homepage, https://github.com/itlabsio/kubedeployer
 Project-URL: Bug Tracker, https://github.com/itlabsio/kubedeployer/issues
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -280,14 +280,20 @@
 ### Options
 
 * __-d__, __-deployer__=smart: structure maintenance types
 (see Supported structure maintenance types);
 * __--dry-run__: only show built manifest without apply it;
 * __--env-file__ list: read in a file of environment variables. If environment
 variable does contain in several files, then it will be has value from last file.
+* __--project-dir \<path\>__: full path to folder with project, if it is not setted,
+used value from environment variable `CI_PROJECT_DIR`, if variable is not setted, as 
+default value used current working directory
+* __--environment \<env_name\>__: environment for builder, if it is not setted, used
+value from environment variable `ENVIRONMENT`
+* __--manifest-folder \<path\>__: path to folder with manifest, path is relative to project_dir. If it is not set, will get value from environment variable `MANIFEST_FOLDER`
 
 ## Supported structure maintenance types
 
 Kubedeployer supports three structure maintenance types of manifests to deploy:
 - orthodox
 - smart - this one is default
 - kustomize
```

