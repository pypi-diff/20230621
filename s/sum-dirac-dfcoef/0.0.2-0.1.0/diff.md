# Comparing `tmp/sum_dirac_dfcoef-0.0.2.tar.gz` & `tmp/sum_dirac_dfcoef-0.1.0.tar.gz`

## Comparing `sum_dirac_dfcoef-0.0.2.tar` & `sum_dirac_dfcoef-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/requirements.txt
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.github/scripts/versionup.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.github/workflows/release-pr.yml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.github/workflows/reusable_test.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/src/sum_dirac_dfcoef/__about__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/src/sum_dirac_dfcoef/__init__.py
--rwxr-xr-x   0        0        0    20035 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/test/.gitignore
--rw-r--r--   0        0        0     9320 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/test/unit_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/test/results/.gitkeep
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/LICENSE
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/README.md
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/requirements.txt
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.github/scripts/versionup.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.github/workflows/release-pr.yml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.github/workflows/reusable_test.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/src/sum_dirac_dfcoef/__about__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/src/sum_dirac_dfcoef/__init__.py
+-rwxr-xr-x   0        0        0    20749 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/test/.gitignore
+-rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/test/integration_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/test/results/.gitkeep
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/PKG-INFO
```

### Comparing `sum_dirac_dfcoef-0.0.2/.github/scripts/versionup.py` & `sum_dirac_dfcoef-0.1.0/.github/scripts/versionup.py`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.0.2/.github/workflows/publish.yml` & `sum_dirac_dfcoef-0.1.0/.github/workflows/publish.yml`

 * *Files 25% similar despite different names*

```diff
@@ -23,14 +23,23 @@
       - name: Build package
         run: |
           hatch build
       - name: Publish package
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
+      - name: Get the tag name
+        id: get_tag_name
+        run: |
+          TAG_NAME=$(echo "${{ github.head_ref }}" | sed -e 's/release-//')
+          echo "tag_name=${TAG_NAME}" >> $GITHUB_ENV
+      - name: Create tag
+        run: |
+          git tag ${{ env.tag_name }}
+          git push origin ${{ env.tag_name }}
       - name: Create release
         uses: actions/create-release@v1
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
-          tag_name: ${{ github.ref }}
-          release_name: ${{ github.ref }}
+          tag_name: ${{ env.tag_name }}
+          release_name: ${{ env.tag_name }}
```

### Comparing `sum_dirac_dfcoef-0.0.2/.github/workflows/release-pr.yml` & `sum_dirac_dfcoef-0.1.0/.github/workflows/release-pr.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: sum_dirac_dfcoef-release-pull-request
+name: create-release-pull-request
 
 on:
   workflow_dispatch:
     inputs:
       major_versionup:
         description: "major version up"
         type: boolean
@@ -59,12 +59,11 @@
       - name: Create Pull request with release-v${{ env.NEW_VERSION }} tag
         run: |
           git config --global user.name "github-actions[bot]"
           git config --global user.email "github-actions[bot]@users.noreply.github.com"
           git checkout -b "${{ env.BRANCH_NAME }}"
           git add .
           git commit -m "Release ${{ env.PACKAGE_NAME }} ${{ env.NEW_VERSION }}"
-          git tag "${{ env.TAG_NAME }}"
           git push origin "${{ env.BRANCH_NAME }}"
           gh pr create --title "Release ${{ env.PACKAGE_NAME }} ${{ env.NEW_VERSION }}" --body "Release ${{ env.PACKAGE_NAME }} ${{ env.NEW_VERSION }}"
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `sum_dirac_dfcoef-0.0.2/.github/workflows/reusable_test.yml` & `sum_dirac_dfcoef-0.1.0/.github/workflows/reusable_test.yml`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.0.2/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py` & `sum_dirac_dfcoef-0.1.0/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python3
 
 import argparse
+from io import TextIOWrapper
+import os
 import re
 import sys
 
 from pymolecule_parser import parse
 
 
 class Atoms:
@@ -81,14 +83,15 @@
         return f"mo_info: {self.mo_info}, mo_energy: {self.mo_energy}, coefficients: {self.data_per_orbital_types}"
 
 
 def parse_args() -> "argparse.Namespace":
     parser = argparse.ArgumentParser(description="Summarize the coefficients from DIRAC output file that *PRIVEC option is used. (c.f. http://www.diracprogram.org/doc/master/manual/analyze/privec.html)")
     parser.add_argument("-i", "--input", type=str, required=True, help="(required) file name of DIRAC output", dest="file")
     parser.add_argument("-m", "--mol", type=str, required=True, help="(required) molecule specification. Write the molecular formula (e.g. Cu2O). ** DON'T write the rational formula (e.g. CH3OH) **")
+    parser.add_argument("-o", "--output", type=str, help="Output file name. Default: (-m or --mol option value).out (e.g) --m H2O => print to H2O.out", dest="output")
     parser.add_argument("-c", "--compress", action="store_true", help="Compress output. Display all coefficients on one line for each MO. This options is useful when you want to use the result in a spreadsheet like Microsoft Excel.", dest="compress")
     parser.add_argument("-t", "--threshold", type=float, default=0.1, help="threshold. Default: 0.1 %% (e.g) --threshold=0.1 => print orbital with more than 0.1 %% contribution", dest="threshold")
     parser.add_argument("-d", "--decimal", type=int, default=5, choices=range(1, 16), help="Set the decimal places. Default: 5 (e.g) --decimal=3 => print orbital with 3 decimal places (0.123, 2.456, ...). range: 1-15", dest="decimal")
     parser.add_argument("-a", "--all-write", action="store_true", help="Print all MOs(Positronic and Electronic).", dest="all_write")
     parser.add_argument("-p", "--positronic-write", action="store_true", help="Print only Positronic MOs.", dest="positronic_write")
     parser.add_argument("--debug", action="store_true", help="print debug output (Normalization constant, Sum of MO coefficient)", dest="debug")
     parser.add_argument("--no-sort", action="store_true", help="Don't sort the output by MO energy")
@@ -144,15 +147,15 @@
 
 
 def space_separated_parsing(line: str) -> "list[str]":
     words = re.split(" +", line.rstrip("\n"))
     return [word for word in words if word != ""]
 
 
-def parse_molecule_input(args: "argparse.Namespace", elements: "list[str]") -> Atoms:
+def parse_molecule_input(args: "argparse.Namespace") -> Atoms:
     """
     Parse the molecule input and return the Atoms object.
 
     """
 
     molecule_dict = parse(args.mol)
     atom_nums = list(molecule_dict.values())  # list of counts of atoms
@@ -338,36 +341,46 @@
 ) -> bool:
     # https://github.com/kohei-noda-qcrg/summarize_dirac_dfcoef_coefficients/issues/7#issuecomment-1377969626
     if len(words) >= 2 and start_vector_print and start_mo_section and not start_mo_coefficients and not is_reading_coefficients:
         return True
     return False
 
 
-def write_results(args: "argparse.Namespace", data_all_mo: "list[Data_per_MO]") -> None:
+def get_output_path(args: "argparse.Namespace") -> str:
+    if args.output is None:
+        output_name = f"{args.mol}.out"
+        output_path = os.path.join(os.getcwd(), output_name)
+    else:
+        output_name = args.output
+        output_path = os.path.abspath(output_name)
+    return output_path
+
+
+def write_results(args: "argparse.Namespace", file: TextIOWrapper, data_all_mo: "list[Data_per_MO]") -> None:
     """
     Write results to stdout
     """
+
     for mo in data_all_mo:
         digit_int = len(str(int(mo.mo_energy)))  # number of digits of integer part
-        print(
-            f"{mo.mo_info} {mo.mo_energy:{digit_int}.{args.decimal}f}",
-            end="" if args.compress else "\n",
-        )
+        # File write but if args.compress is True \n is not added
+        mo_info_energy = f"{mo.mo_info} {mo.mo_energy:{digit_int}.{args.decimal}f}" + ("\n" if not args.compress else "")
+        file.write(mo_info_energy)
 
         d: Data_per_orbital_types
         for d in mo.data_per_orbital_types:
             if args.compress:
                 orb_type = str(d.orbital_type)
                 output_str = f" {orb_type} {d.mo_percentage:.{args.decimal}f}"
-                print(output_str, end="")
+                file.write(output_str)
             else:
                 orb_type = str(d.orbital_type).ljust(11, " ")
-                output_str = f"{orb_type} {d.mo_percentage:{args.decimal+4}.{args.decimal}f} %"
-                print(output_str)
-        print()  # "\n"
+                output_str = f"{orb_type} {d.mo_percentage:{args.decimal+4}.{args.decimal}f} %\n"
+                file.write(output_str)
+        file.write("\n")  # add empty line
         debug_print_wrapper(args, f"Normalization constant is {mo.norm_constant:.{args.decimal}f}")
         debug_print_wrapper(args, f"sum of coefficient {mo.sum_coefficients:.{args.decimal}f}")
 
 
 def main() -> None:
     start_mo_coefficients: bool = False
     start_mo_section: bool = False
@@ -380,15 +393,15 @@
     coefficients: Coefficients = Coefficients()
     # fmt: off
     elements: "list[str]" = ["H", "He", "Li", "Be", "B", "C", "N", "O", "F", "Ne", "Na", "Mg", "Al", "Si", "P", "S", "Cl", "Ar", "K", "Ca", "Sc", "Ti", "V", "Cr", "Mn", "Fe", "Co", "Ni", "Cu", "Zn", "Ga", "Ge", "As", "Se", "Br", "Kr", "Rb", "Sr", "Y", "Zr", "Nb", "Mo", "Tc", "Ru", "Rh", "Pd", "Ag", "Cd", "In", "Sn", "Sb", "Te", "I", "Xe", "Cs", "Ba", "La", "Ce", "Pr", "Nd", "Pm", "Sm", "Eu", "Gd", "Tb", "Dy", "Ho", "Er", "Tm", "Yb", "Lu", "Hf", "Ta", "W", "Re", "Os", "Ir", "Pt", "Au", "Hg", "Tl", "Pb", "Bi", "Po", "At", "Rn", "Fr", "Ra", "Ac", "Th", "Pa", "U", "Np", "Pu", "Am", "Cm", "Bk", "Cf", "Es", "Fm", "Md", "No", "Lr", "Rf", "Db", "Sg", "Bh", "Hs", "Mt", "Ds", "Rg"]
     # fmt: on
 
     args: "argparse.Namespace" = parse_args()
     dirac_file: str = get_dirac_filename(args)
-    atoms: Atoms = parse_molecule_input(args, elements)
+    atoms: Atoms = parse_molecule_input(args)
 
     data_all_electronic_mo: "list[Data_per_MO]" = []
     data_all_positronic_mo: "list[Data_per_MO]" = []
     with open(dirac_file, encoding="utf-8") as f:
         for line in f:
             words: "list[str]" = space_separated_parsing(line)
             if not start_vector_print:
@@ -468,16 +481,19 @@
             # Read coefficients or the end of coefficients section
             elif start_mo_coefficients:
                 if not is_this_row_for_coefficients(words):
                     continue
                 is_reading_coefficients = True
                 get_coefficient(words, atoms, coefficients, elements)
     # End of reading file
+    output_path = get_output_path(args)
+    file = open(output_path, "w")
     if args.all_write or args.positronic_write:
         if not args.no_sort:
             data_all_positronic_mo.sort(key=lambda x: x.mo_energy)
-        write_results(args, data_all_positronic_mo)
-        print()  # Add a blank line
+        write_results(args, file, data_all_positronic_mo)
+        file.write("\n")  # Add a blank line
     if args.all_write or not args.positronic_write:  # Electronic
         if not args.no_sort:
             data_all_electronic_mo.sort(key=lambda x: x.mo_energy)
-        write_results(args, data_all_electronic_mo)
+        write_results(args, file, data_all_electronic_mo)
+    file.close()
```

### Comparing `sum_dirac_dfcoef-0.0.2/test/unit_test.py` & `sum_dirac_dfcoef-0.1.0/test/integration_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,26 +41,23 @@
     os.chdir(test_path)
     print(test_path, " test start...")
 
     ref_filepath = os.path.join(test_path, "data", ref_filename)
     result_filepath = os.path.join(test_path, "results", result_filename)
     input_filepath = os.path.join(test_path, "data", input_filename)
 
-    test_command = f"sum_dirac_dfcoef -m {mol} -i {input_filepath} {options}"
+    test_command = f"sum_dirac_dfcoef -m {mol} -i {input_filepath} -o {result_filepath} {options}"
     print(test_command)
-    with open(result_filepath, "w") as file_output:
-        process = subprocess.run(
-            test_command,
-            shell=True,
-            stdout=file_output,
-            encoding="utf-8",
-            stderr=file_output,
-        )
-        if process.returncode != 0:
-            sys.exit(f"{test_command} failed with return code {process.returncode}")
+    process = subprocess.run(
+        test_command,
+        shell=True,
+        encoding="utf-8",
+    )
+    if process.returncode != 0:
+        sys.exit(f"{test_command} failed with return code {process.returncode}")
 
     ref_file: "list[list[str]]" = [re.split(" +", line.rstrip("\n")) for line in list(filter(lambda val: val != "", open(ref_filepath, "r").read().splitlines()))]
     out_file: "list[list[str]]" = [re.split(" +", line.rstrip("\n")) for line in list(filter(lambda val: val != "", open(result_filepath, "r").read().splitlines()))]
     # File should have the same number of lines
     assert len(ref_file) == len(out_file), f"Number of lines in {ref_filename}(={len(ref_file)}) and {result_filename}(={len(out_file)}) are different."
     threshold: float = 1e-10
     checked = len(ref_file)
@@ -104,26 +101,23 @@
     os.chdir(test_path)
     print(test_path, " test start...")
 
     ref_filepath = os.path.join(test_path, "data", ref_filename)
     result_filepath = os.path.join(test_path, "results", result_filename)
     input_filepath = os.path.join(test_path, "data", input_filename)
 
-    test_command = f"sum_dirac_dfcoef -m {mol} -i {input_filepath} {options}"
+    test_command = f"sum_dirac_dfcoef -m {mol} -i {input_filepath} -o {result_filepath} {options}"
     print(test_command)
-    with open(result_filepath, "w") as file_output:
-        process = subprocess.run(
-            test_command,
-            shell=True,
-            stdout=file_output,
-            encoding="utf-8",
-            stderr=file_output,
-        )
-        if process.returncode != 0:
-            sys.exit(f"{test_command} failed with return code {process.returncode}")
+    process = subprocess.run(
+        test_command,
+        shell=True,
+        encoding="utf-8",
+    )
+    if process.returncode != 0:
+        sys.exit(f"{test_command} failed with return code {process.returncode}")
 
     ref_file: "list[list[str]]" = [re.split(" +", line.rstrip("\n")) for line in list(filter(lambda val: val != "", open(ref_filepath, "r").read().splitlines()))]
     out_file: "list[list[str]]" = [re.split(" +", line.rstrip("\n")) for line in list(filter(lambda val: val != "", open(result_filepath, "r").read().splitlines()))]
     # File should have the same number of lines
     assert len(ref_file) == len(out_file), f"Number of lines in {ref_filename}(={len(ref_file)}) and {result_filename}(={len(out_file)}) are different."
     threshold: float = 1e-10
     checked = len(ref_file)
```

### Comparing `sum_dirac_dfcoef-0.0.2/.gitignore` & `sum_dirac_dfcoef-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.0.2/LICENSE` & `sum_dirac_dfcoef-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.0.2/README.md` & `sum_dirac_dfcoef-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,24 @@
 ```
 
 ## Usage
 
 You can use this program with the following command!
 
 ```sh
-/path/to/sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME
+# Output to MOLECULE_NAME.out
+sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME
+# Specify output file name with -o option
+sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME -o OUTPUT_FILE_NAME
 ```
 
 (e.g.)
 
 ```sh
-./sum_dirac_dfcoef -i x2c_uo2_238.out -m UO2
+sum_dirac_dfcoef -i x2c_uo2_238.out -m UO2
 ```
 
 A part of x2c_uo2_238.out (DIRAC output file, ... represents an omission)
 
 ```out
 ...
     **************************************************************************
@@ -111,14 +114,17 @@
   (required) file name of DIRAC output
 
 - -m MOL, --mol MOL
 
   (required) molecule specification. Write the molecular formula (e.g. Cu2O).  
   **DON'T write the rational formula (e.g. CH3OH)**
 
+-  -o OUTPUT, --output OUTPUT
+  Output file name. Default: (-m or --mol option value).out (e.g) --m H2O => print to H2O.out
+
 - -c, --compress
 
   Compress output. Display all coefficients on one line for each MO.  
   This options is useful when you want to use the result in a spreadsheet like Microsoft Excel.
 
 - -t THRESHOLD, --threshold THRESHOLD
 
@@ -126,14 +132,20 @@
   (e.g) --threshold=0.1 => print orbital with more than 0.1 % contribution
 
 - -d DECIMAL, --decimal DECIMAL
 
   Set the decimal places. Default: 5  
   (e.g) --decimal=3 => print orbital with 3 decimal places (0.123, 2.456, ...). range: 1-15
 
+- -a, --all-write
+  Print all MOs(Positronic and Electronic).
+
+- -p, --positronic-write
+  Print only Positronic MOs.
+
 - --debug
 
   print debug output (Normalization constant, Sum of MO coefficient)
 
 - --no-sort
 
   Don't sort the output by MO energy
```

### Comparing `sum_dirac_dfcoef-0.0.2/pyproject.toml` & `sum_dirac_dfcoef-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.0.2/PKG-INFO` & `sum_dirac_dfcoef-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sum_dirac_dfcoef
-Version: 0.0.2
+Version: 0.1.0
 Summary: This is a utility to summarize the contribution of each atomic orbital per molecular orbital from the DIRAC output file that the *PRIVEC and .VECPRI options are used.
 Project-URL: Documentation, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef#readme
 Project-URL: Issues, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef/issues
 Project-URL: Source, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef
 Author-email: Kohei Noda <kohei-noda@hiroshima-u.ac.jp>
 License-Expression: MIT
 License-File: LICENSE
@@ -40,21 +40,24 @@
 ```
 
 ## Usage
 
 You can use this program with the following command!
 
 ```sh
-/path/to/sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME
+# Output to MOLECULE_NAME.out
+sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME
+# Specify output file name with -o option
+sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME -o OUTPUT_FILE_NAME
 ```
 
 (e.g.)
 
 ```sh
-./sum_dirac_dfcoef -i x2c_uo2_238.out -m UO2
+sum_dirac_dfcoef -i x2c_uo2_238.out -m UO2
 ```
 
 A part of x2c_uo2_238.out (DIRAC output file, ... represents an omission)
 
 ```out
 ...
     **************************************************************************
@@ -135,14 +138,17 @@
   (required) file name of DIRAC output
 
 - -m MOL, --mol MOL
 
   (required) molecule specification. Write the molecular formula (e.g. Cu2O).  
   **DON'T write the rational formula (e.g. CH3OH)**
 
+-  -o OUTPUT, --output OUTPUT
+  Output file name. Default: (-m or --mol option value).out (e.g) --m H2O => print to H2O.out
+
 - -c, --compress
 
   Compress output. Display all coefficients on one line for each MO.  
   This options is useful when you want to use the result in a spreadsheet like Microsoft Excel.
 
 - -t THRESHOLD, --threshold THRESHOLD
 
@@ -150,14 +156,20 @@
   (e.g) --threshold=0.1 => print orbital with more than 0.1 % contribution
 
 - -d DECIMAL, --decimal DECIMAL
 
   Set the decimal places. Default: 5  
   (e.g) --decimal=3 => print orbital with 3 decimal places (0.123, 2.456, ...). range: 1-15
 
+- -a, --all-write
+  Print all MOs(Positronic and Electronic).
+
+- -p, --positronic-write
+  Print only Positronic MOs.
+
 - --debug
 
   print debug output (Normalization constant, Sum of MO coefficient)
 
 - --no-sort
 
   Don't sort the output by MO energy
```

