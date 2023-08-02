# Comparing `tmp/uranie-launcher-1.0.1.tar.gz` & `tmp/uranie-launcher-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/catB/cs270042/travail/uranie/new/dist/tmp33455j71/uranie-launcher-1.0.1.tar", last modified: Thu Jul  6 14:06:40 2023, max compression
+gzip compressed data, was "/volatile/catA/rl222169/rn/uranie/u2/dist/tmp5m8i90b6/uranie-launcher-2.0.0.tar", last modified: Wed Aug  2 15:16:28 2023, max compression
```

## Comparing `uranie-launcher-1.0.1.tar` & `uranie-launcher-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwx------   0 cs270042 (270042) dm2s-user-cat-b (470573)        0 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/
-drwx------   0 cs270042 (270042) dm2s-user-cat-b (470573)        0 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/src/
-drwx------   0 cs270042 (270042) dm2s-user-cat-b (470573)        0 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/src/uranie_launcher/
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)        6 2023-07-06 14:04:53.000000 uranie-launcher-1.0.1/src/uranie_launcher/VERSION
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)      405 2023-06-28 09:14:58.000000 uranie-launcher-1.0.1/src/uranie_launcher/__init__.py
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)    11882 2023-07-06 08:21:08.000000 uranie-launcher-1.0.1/src/uranie_launcher/_data_2_uranie.py
--rwx------   0 cs270042 (270042) dm2s-user-cat-b (470573)     1614 2023-06-29 12:25:45.000000 uranie-launcher-1.0.1/src/uranie_launcher/_rootlogon.py
--rwx------   0 cs270042 (270042) dm2s-user-cat-b (470573)     2346 2023-07-06 08:30:15.000000 uranie-launcher-1.0.1/src/uranie_launcher/_run_unitary.py
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)     8656 2023-06-28 09:14:58.000000 uranie-launcher-1.0.1/src/uranie_launcher/execution.py
--rwx------   0 cs270042 (270042) dm2s-user-cat-b (470573)     3229 2023-06-29 08:31:50.000000 uranie-launcher-1.0.1/src/uranie_launcher/launcher.py
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)     9272 2023-07-06 12:35:34.000000 uranie-launcher-1.0.1/src/uranie_launcher/uncertainty_data.py
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)      819 2023-06-28 09:14:58.000000 uranie-launcher-1.0.1/src/uranie_launcher/utils.py
-drwx------   0 cs270042 (270042) dm2s-user-cat-b (470573)        0 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/src/uranie_launcher.egg-info/
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)     1340 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/src/uranie_launcher.egg-info/PKG-INFO
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)      603 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/src/uranie_launcher.egg-info/SOURCES.txt
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)        1 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/src/uranie_launcher.egg-info/dependency_links.txt
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)      162 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/src/uranie_launcher.egg-info/entry_points.txt
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)       28 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/src/uranie_launcher.egg-info/requires.txt
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)       16 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/src/uranie_launcher.egg-info/top_level.txt
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)    35149 2023-06-28 09:15:00.000000 uranie-launcher-1.0.1/LICENSE
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)      856 2023-07-03 07:57:44.000000 uranie-launcher-1.0.1/README.md
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)       81 2023-06-28 09:14:58.000000 uranie-launcher-1.0.1/pyproject.toml
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)     1580 2023-07-06 13:49:06.000000 uranie-launcher-1.0.1/setup.py
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)     1340 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/PKG-INFO
--rw-------   0 cs270042 (270042) dm2s-user-cat-b (470573)       38 2023-07-06 14:06:40.000000 uranie-launcher-1.0.1/setup.cfg
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/src/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/src/uranie_launcher/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    13051 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/src/uranie_launcher/data.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    12142 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/src/uranie_launcher/execution.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10579 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/src/uranie_launcher/input_data.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1088 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/src/uranie_launcher/utils.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      962 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/src/uranie_launcher/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    12423 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/src/uranie_launcher/_data_2_uranie.py
+-rwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)     2257 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/src/uranie_launcher/_run_unitary.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-08-02 15:14:20.000000 uranie-launcher-2.0.0/src/uranie_launcher/VERSION
+-rwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)     2847 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/src/uranie_launcher/launcher.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/src/uranie_launcher.egg-info/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       28 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/src/uranie_launcher.egg-info/requires.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       16 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/src/uranie_launcher.egg-info/top_level.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      591 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/src/uranie_launcher.egg-info/SOURCES.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      162 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/src/uranie_launcher.egg-info/entry_points.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/src/uranie_launcher.egg-info/dependency_links.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1340 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/src/uranie_launcher.egg-info/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/pyproject.toml
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1580 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/setup.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      856 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/README.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    35149 2023-08-02 15:12:21.000000 uranie-launcher-2.0.0/LICENSE
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1340 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-08-02 15:16:28.000000 uranie-launcher-2.0.0/setup.cfg
```

### Comparing `uranie-launcher-1.0.1/src/uranie_launcher/_data_2_uranie.py` & `uranie-launcher-2.0.0/src/uranie_launcher/_data_2_uranie.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,238 +1,249 @@
 """Contains the implementation of the functions used in launcher.py
 """
 import json
 import os
 from pathlib import Path
-from typing import Dict, List
-from . import _rootlogon, utils, uncertainty_data, execution as exe
+from typing import Dict, List, Tuple
+
+from URANIE import DataServer, Launcher, Sampler
+import ROOT
+
+from . import utils, input_data, execution as exe
 
 URANIE_TCODE_LAUNCHER = "uranie-launcher-unitary"
-URANIE_TCODE_JSON = ".uranie-unitary-commands.json"
+URANIE_TCODE_JSON = ".uranie-launcher-commands.json"
 
-STUDY_EXP_DESIGN = "experimental_design.dat"
-STUDY_WORKDIR_NAME = "uranie_unitaries"
-STUDY_OUTFILE_NAME = "aggregated_outputs.dat"
-STUDY_OUTFILE_NAME_FAILED = "aggregated_outputs_failed.dat"
+URANIE_FAILED_VALUE = "1.234567890e+00"
+"""This is the default value used by Uranie when calculation failed."""
 
 
-def create_data_server(outputs: uncertainty_data.Outputs):
+def create_data_server(outputs: input_data.Outputs) -> DataServer.TDataServer:
     """Create the data server for Uranie
 
     Parameters
     ----------
-    outputs : uncertainty_data.Outputs
+    outputs : input_data.Outputs
         Object containing the name of the outputs and all the informations about them.
 
     Returns
     -------
-    _rootlogon.DataServer.TDataServer
+    DataServer.TDataServer
         TDataServer object.
     """
 
-    title = f"Quantities: {[output.quantity_of_interest for output in outputs.outputs]}"
-    return _rootlogon.DataServer.TDataServer(outputs.name, title)
+    title = f"Quantities = {[output.quantity_of_interest for output in outputs.outputs]}"
+    return DataServer.TDataServer(outputs.name, title)
 
 
-def set_inputs(inputs: uncertainty_data.Inputs, t_data_server: _rootlogon.DataServer.TDataServer):
+def set_inputs(inputs: input_data.Inputs, t_data_server: DataServer.TDataServer):
     """Defines the parameters of the distribution law for each uncertains values,
     and associate the variable_name to the flag used in file_flag.
 
     Parameters
     ----------
-    inputs : uncertainty_data.Inputs
+    inputs : input_data.Inputs
         Object containing all the infos about the uncertain parameters.
-    t_data_server : _rootlogon.DataServer.TDataServer
+    t_data_server : DataServer.TDataServer
         A TDataServer object
 
     Raises
     ------
     ValueError
         Invalid distribution type if the variable distribution isn't 'Uniform' or 'TruncatedNormal'.
     """
     for _input in inputs.inputs:
         variable_name = _input.variable_name
-        if isinstance(_input.distribution, uncertainty_data.Inputs.DistributionUniform):
-            t_data_server.addAttribute(_rootlogon.DataServer.TUniformDistribution(
+        if isinstance(_input.distribution, input_data.Inputs.DistributionUniform):
+            t_data_server.addAttribute(DataServer.TUniformDistribution(
                 variable_name, _input.distribution.lower_bound, _input.distribution.upper_bound))
 
-        elif isinstance(_input.distribution, uncertainty_data.Inputs.DistributionTruncatedNormal):
+        elif isinstance(_input.distribution, input_data.Inputs.DistributionTruncatedNormal):
             mean = _input.distribution.mean
             std_dev = _input.distribution.standard_deviation
-            t_data_server.addAttribute(_rootlogon.DataServer.TNormalDistribution(variable_name,
-                                                                                 mean,
-                                                                                 std_dev))
-            t_data_server.getAttribute(variable_name).setBounds(_input.distribution.lower_bound,
-                                                                _input.distribution.upper_bound)
+            t_data_server.addAttribute(DataServer.TNormalDistribution(
+                variable_name, mean, std_dev))
+            t_data_server.getAttribute(variable_name).setBounds(
+                _input.distribution.lower_bound, _input.distribution.upper_bound)
 
         else:
             raise ValueError("Invalid distribution type: "
                              f"{_input.distribution.__class__.__name__}")
 
         t_data_server.getAttribute(variable_name).setFileFlag(str(inputs.file_flag), _input.flag)
 
 
-def generate_sample(propagation: uncertainty_data.Propagation,
-                    t_data_server: _rootlogon.DataServer.TDataServer,
-                    output_dirname: Path):
+def generate_sample(propagation: input_data.Propagation,
+                    outputs: input_data.Outputs,
+                    t_data_server: DataServer.TDataServer,
+                    output_directory: Path
+                    ) -> Sampler.TQMC or Sampler.TSampling:
     """Definition of the experimental plan
 
     Parameters
     ----------
-    propagation : uncertainty_data.Propagation
+    propagation : input_data.Propagation
         Object containing the name of the propagation method used and the sample size.
-    t_data_server : _rootlogon.DataServer.TDataServer
+    outputs : input_data.Outputs
+        Object containing the name of the experimental design file name.
+    t_data_server : DataServer.TDataServer
         A TDataServer object
-    output_dirname: Path
+    output_directory: Path
         Name of the directory where are stored the results
         of the uncertainty quantification calculation
     Returns
     -------
-    _rootlogon.Sampler.TQMC or _rootlogon.Sampler.TSampling
+    Sampler.TQMC or Sampler.TSampling
         t_sampler object containing the experimental plan.
 
     Raises
     ------
     ValueError
         Invalid sampling method if the sampling method is not 'SRS' or 'Sobol'.
     """
     if propagation.sampling_method == propagation.SOBOL:
         # here I considered that canvas was deterministic
-        t_sampler = _rootlogon.Sampler.TQMC(
+        t_sampler = Sampler.TQMC(
             t_data_server, propagation.sampling_method, propagation.sample_size)
     elif propagation.sampling_method == propagation.SRS:
-        t_sampler = _rootlogon.Sampler.TSampling(
+        t_sampler = Sampler.TSampling(
             t_data_server, propagation.sampling_method, propagation.sample_size)
     else:
         raise ValueError(f"Unknown sampling method: {propagation.sampling_method}")
 
     t_sampler.generateSample()
 
-    t_data_server.exportData(str(output_dirname / STUDY_EXP_DESIGN))
+    t_data_server.exportData(str(output_directory / outputs.experimental_design_filename))
 
     return t_sampler
 
 
-def visualisation(t_data_server: _rootlogon.DataServer.TDataServer):
+def visualisation(t_data_server: DataServer.TDataServer):  # pragma: no cover
     """Plot a graph if the visualization variable is equal to True
 
     Parameters
     ----------
-    t_data_server : _rootlogon.DataServer.TDataServer
+    t_data_server : DataServer.TDataServer
         A TDataServer object
     """
-    _rootlogon.ROOT.gROOT.SetBatch(False)  # pylint: disable=no-member
-    canvas = _rootlogon.ROOT.TCanvas()  # pylint: disable=no-member
+    ROOT.gROOT.SetBatch(False)  # pylint: disable=no-member
+    canvas = ROOT.TCanvas()  # pylint: disable=no-member
     canvas.Clear()
     t_data_server.drawPairs()
     canvas.Draw()
 
 
-def set_outputs(outputs: uncertainty_data.Outputs, unitary_result_filename: str):
+def set_outputs(outputs: input_data.Outputs) -> List[Launcher.TOutputFileRow]:
     """Prepares the unitary aggregated outputs file.
 
     Parameters
     ----------
-    outputs : uncertainty_data.Outputs
+    outputs : input_data.Outputs
         Object containing the name of the outputs and all the informations about them.
-    unitary_result_filename : str
-        Name of the file containing the result of the
-        aggregations functions for an unitary calculation
 
     Returns
     -------
-    _rootlogon.Launcher.TOutputFileRow
-        File that will contain the unitary aggregated outputs
-    List
-        Names of the different aggregations functions
+    List[Launcher.TOutputFileRow]
+        List of file that will contain the unitary aggregated outputs
     """
-    # The output file of the code
-    t_output_file = _rootlogon.Launcher.TOutputFileRow(unitary_result_filename)
+    # The output files of the code
+    t_output_files = []
 
     # The attribute in the output file
-    # FIXME : here, headers is a list containing ALL the headers of all outputs.
-    # May not be a good idea to do so...
-    headers = []
     for output in outputs.outputs:
+        t_output_file = Launcher.TOutputFileRow(output.filename)
         for header in output.headers:
-            headers.append(header)
-            t_output_file.addAttribute(_rootlogon.DataServer.TAttribute(header))
-
-
-    return t_output_file, headers
+            t_output_file.addAttribute(DataServer.TAttribute(header))
+        t_output_files.append(t_output_file)
+    return t_output_files
 
 
 def create_launcher(commands_to_execute: Dict[str, List],
-                    t_data_server: _rootlogon.DataServer.TDataServer,
-                    output_dirname: Path,
-                    t_output_file: _rootlogon.Launcher.TOutputFileRow):
+                    t_data_server: DataServer.TDataServer,
+                    output_directory: Path,
+                    t_output_files: List[Launcher.TOutputFileRow]
+                    ) -> Launcher.TLauncher:
     """Create the launcher for Uranie
 
     Parameters
     ----------
     commands_to_execute : Dict[str, List]
         Name of the script or the command which URANIE will execute with all its arguments.
-    t_data_server : _rootlogon.DataServer.TDataServer
+    t_data_server : DataServer.TDataServer
         A TDataServer object
-    output_dirname : Path
+    output_directory : Path
         Name of the directory where are stored the results
         of the uncertainty quantification calculation
-    t_output_file : _rootlogon.Launcher.TOutputFileRow
-        File that will contain the unitary aggregated outputs
+    t_output_files : List[Launcher.TOutputFileRow]
+        List of files that will contain the unitary aggregated outputs
 
     Returns
     -------
-    _rootlogon.Launcher.TLauncher
+    Launcher.TLauncher
         t_launcher object.
-    Path
-        Directory where all unitary calculations are stored.
     """
-    commands_json_file = output_dirname / URANIE_TCODE_JSON
-    with open(commands_json_file, 'w', encoding = 'utf-8') as tcode_file:
+    commands_json_file = output_directory / URANIE_TCODE_JSON
+    with open(commands_json_file, 'w', encoding='utf-8') as tcode_file:
         json.dump(commands_to_execute, tcode_file, indent=4)
 
-    command = f'{URANIE_TCODE_LAUNCHER} {commands_json_file} > log.out 2> log.err'
-    t_code = _rootlogon.Launcher.TCode(t_data_server, command)
+    command = [URANIE_TCODE_LAUNCHER, str(commands_json_file), "> log.out 2> log.err"]
+    if utils.get_log_level() >= utils.DEBUG:
+        command.insert(1, "--debug")
+    t_code = Launcher.TCode(t_data_server, " ".join(command))
 
     # we add the output file of the code
-    t_code.addOutputFile(t_output_file)
-
-    uranie_work_dir = output_dirname / STUDY_WORKDIR_NAME
+    for t_output_file in t_output_files:
+        t_code.addOutputFile(t_output_file)
 
-    t_launcher = _rootlogon.Launcher.TLauncher(t_data_server, t_code)
-    # To back up all directories
-    t_launcher.setSave()
-    t_launcher.setClean()
-    t_launcher.setWorkingDirectory(str(uranie_work_dir))
-
-    return t_launcher, uranie_work_dir
+    return Launcher.TLauncher(t_data_server, t_code)
 
 
 def run_calculations(execution: exe.Execution,
-                     t_launcher: _rootlogon.Launcher.TLauncher):
+                     t_launcher: Launcher.TLauncher,
+                     output_directory: Path) -> Path:
     """Launch the calculation according to the appropriate mode (on your desktop or on a cluster).
 
     Parameters
     ----------
     execution: execution.Execution
         Object containing all the infos about how to execute the calculations.
-    t_launcher : _rootlogon.Launcher.TLauncher
+    t_launcher : Launcher.TLauncher
         t_launcher object.
+    output_directory : Path
+        Name of the directory where are stored the results
+        of the uncertainty quantification calculation
 
     Raises
     ------
     ValueError
         Invalid execution mode if it's different from 'desktop' or 'cluster'.
+    ValueError
+        execution.clean and output_directory == execution.working_directory is not possible.
     """
+
+    # To back up all directories
+    t_launcher.setSave(execution.save)
+    t_launcher.setClean(execution.clean)
+
+    # Uranie working directory
+    t_launcher.setWorkingDirectory(str(execution.working_directory))
+
+    if output_directory == execution.working_directory and execution.clean:
+        raise ValueError(
+            "execution.clean is True and output_directory == "
+            "execution.working_directory is not possible.")
+
     if isinstance(execution, exe.ExecutionLocal):
         if execution.nb_jobs == 1:  # Launching code on a single processor
             # For display during runing
-            if execution.visualization:
-                t_launcher.setVarDraw("max:initial_power","","") # FIXME lie a integration_bench
-        t_launcher.run(f"localhost={execution.nb_jobs}")
+            if execution.visualization:  # pragma: no cover
+                t_launcher.setVarDraw("max:initial_power", "", "")  # FIXME lie a integration_bench
+            t_launcher.run()
+        else:
+            t_launcher.run(f"localhost={execution.nb_jobs}")
 
     # elif isinstance(execution, exe.ExecutionSlurm):
     #     pass
     #     #sbatch -n <nb de tâches> -c <nb de cœurs par tâche> -p <partition> --qos=<qos>
     #     # -A <account> -t <walltime HH:MM:SS> -J <jobname> -o <fichier de sortie>
     #     # -e <fichier d’erreur> --mail-user=<email> --mail-type=<BEGIN|END|FAIL|ALL>
     #     # -w <liste des nœuds> myscript.sh
@@ -249,62 +260,77 @@
         Absoulut path to the URANIE output directory.
     unitary_result_filename : str
         Name of the file containing the result of the
         aggregations functions for an unitary calculation
 
     Returns
     -------
-    nb_fail : int
+    int
         Number of failed calculations.
     """
     list_directories = os.listdir(uranie_work_dir)
     list_directories.remove('UranieResults')
     nb_fail = 0
     for directory in list_directories:
         uranie_results_file = uranie_work_dir / directory / unitary_result_filename
+        utils.debug(f"Check output {uranie_results_file}: {uranie_results_file.is_file()}")
         if not uranie_results_file.is_file():
             nb_fail += 1
 
     return nb_fail
 
 
-def save_calculations(propagation: uncertainty_data.Propagation,
-                      t_data_server: _rootlogon.DataServer.TDataServer,
-                      headers: List,
-                      output_dirname: Path,
-                      unitary_result_filename: str,
-                      uranie_work_dir: Path):
+def save_calculations(propagation: input_data.Propagation,
+                      execution: exe.Execution,
+                      outputs: input_data.Outputs,
+                      t_data_server: DataServer.TDataServer,
+                      output_directory: Path) -> Tuple[Path, int]:
     """Save calculation results in one file for valid calculations,
     and in another for failed calculations (if there is some).
 
     Parameters
     ----------
-    propagation : uncertainty_data.Propagation
+    propagation : input_data.Propagation
         Object containing the name of the propagation method used.
-    t_data_server : _rootlogon.DataServer.TDataServer
+    execution: execution.Execution
+        Object containing all the infos about how to execute the calculations.
+    outputs : input_data.Outputs
+        Object containing the outputs of the study to recover output filename.
+    t_data_server : DataServer.TDataServer
         A TDataServer object.
-    headers : List
-        Names of the different aggregations functions
-    output_dirname: Path
+    output_directory: Path
         Name of the directory where are stored the results
         of the uncertainty quantification calculation
-    unitary_result_filename : str
-        Name of the file containing the result of the
-        aggregations functions for an unitary calculation
-    uranie_work_dir
-        Directory where all unitary calculations are stored.
+
+    Returns
+    -------
+    Tuple[Path, int]
+        Path to output file defined as ``output_directory/outputs.output_filename``
+        and nb of failed.
     """
-    # "1.234567890e+00" is the default value used by Uranie when calculation failed.
-    nb_fail = _count_of_failed_calculations(uranie_work_dir, unitary_result_filename)
 
+    output0 = outputs.outputs[0]
+    nb_fail = _count_of_failed_calculations(execution.working_directory, output0.filename)
+
+    ascii_filepath = output_directory / outputs.output_filename
+
+    # Some succeded
     if nb_fail < propagation.sample_size:
-        t_data_server.exportData(str(output_dirname/STUDY_OUTFILE_NAME), "*",
-                                 f"{headers[0]}!=1.234567890e+00")
+        t_data_server.exportData(
+            str(ascii_filepath), "*", f"{output0.headers[0]}!={URANIE_FAILED_VALUE}")
+
+    if utils.get_log_level() >= utils.INFO:
+        t_data_server.scan()
 
+    # Some failed
     if nb_fail > 0:
-        t_data_server.exportData(str(output_dirname/STUDY_OUTFILE_NAME_FAILED), "*",
-                                 f"{headers[0]}==1.234567890e+00")
         utils.info(f"\033[1;31m{nb_fail} over {propagation.sample_size} calculation(s) "
                    "failed !\033[0m")
-    elif nb_fail == 0:
+        utils.debug(f"export failed simulations to {output_directory/outputs.failed_filename}.")
+        utils.debug(f" -> condition: {output0.headers[0]}=={URANIE_FAILED_VALUE}")
+        t_data_server.exportData(str(output_directory/outputs.failed_filename), "*",
+                                 f"{output0.headers[0]}=={URANIE_FAILED_VALUE}")
+    else:
         utils.info(f"\033[1;32mAll the {propagation.sample_size} calculation(s) "
                    "have succeeded !\033[0m")
+
+    return ascii_filepath, nb_fail
```

### Comparing `uranie-launcher-1.0.1/src/uranie_launcher/_run_unitary.py` & `uranie-launcher-2.0.0/src/uranie_launcher/_run_unitary.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,59 +6,63 @@
 import subprocess
 import sys
 import argparse
 from pathlib import Path
 from uranie_launcher import __name__ as uranie_launcher_name
 from uranie_launcher import utils
 
+
 def main_unitary(arguments):
     """ Run the unitary function with the given command line arguments.
 
     Parameters
     ----------
     arguments: list of str
         Command line arguments.
 
     Returns
     -------
     int
         Return code.
     """
     # Interpret arguments
-    parser = argparse.ArgumentParser(description = __doc__)
+    parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument(
         "commands_json_file",
-        help = "Name of the script or the command to execute")
+        help="Name of the script or the command to execute")
+    parser.add_argument(
+        "--debug",
+        action="store_true",
+        help="activate debug mode (default: %(default)s)")
     args = parser.parse_args(arguments)
 
-    with open(args.commands_json_file, encoding = 'utf-8') as f:
+    utils.set_verbosity(utils.DEBUG if args.debug else utils.INFO)
+
+    with open(args.commands_json_file, encoding='utf-8') as f:
         commands = json.load(f)
 
     for _command, _arguments in commands.items():
-        try:
-            proc = subprocess.run([_command] + _arguments,
-                                stdout = subprocess.PIPE,
-                                stderr = subprocess.PIPE,
-                                check = True)
-            utils.info(f"{Path(__file__).name} : Start the execution of the command "
-                       f"subprocess.run({[_command] + _arguments})")
-            utils.info(f"{Path(__file__).name} : proc.stdout:")
-            utils.info(proc.stdout.decode(encoding = 'utf-8'))
-            utils.info(f"{Path(__file__).name} : proc.stderr:")
-            utils.info(proc.stderr.decode(encoding = 'utf-8'))
-            if proc.returncode == 0:
-                utils.info(f"{Path(__file__).name} : The execution of the command "
-                           f"subprocess.run({[_command] + _arguments}) was successful.")
-            else:
-                utils.info(f"{Path(__file__).name} : Failed to execute the command "
-                           f"subprocess.run({[_command] + _arguments})\n"
-                           f"{proc.stdout.decode(encoding = 'utf-8')} {proc.returncode}")
-                return proc.returncode
-        except subprocess.CalledProcessError:
-            return 1
+        utils.info(f"{Path(__file__).name} : Start the execution of the command "
+                   f"subprocess.run({[_command] + _arguments})")
+        proc = subprocess.run([_command] + _arguments,  # pylint: disable=subprocess-run-check
+                              stdout=subprocess.PIPE,
+                              stderr=subprocess.PIPE)
+
+        utils.info(f"{_command} : proc.stdout:")
+        utils.info(proc.stdout.decode(encoding='utf-8'))
+        utils.info(f"{_command} : proc.stderr:")
+        utils.info(proc.stderr.decode(encoding='utf-8'))
+        if proc.returncode == 0:
+            utils.info(f"The execution of the command "
+                       f"subprocess.run({[_command] + _arguments}) was successful.")
+        else:
+            utils.info(f"Failed to execute the command "
+                       f"subprocess.run({[_command] + _arguments}). Returned {proc.returncode}.")
+            return proc.returncode
 
     return 0
 
+
 def run_unitary():
     """ Entry point for the ``uranie-launcher-unitary`` script."""
     logging.getLogger(uranie_launcher_name).addHandler(logging.StreamHandler(sys.stdout))
     sys.exit(main_unitary(sys.argv[1:]))
```

### Comparing `uranie-launcher-1.0.1/src/uranie_launcher/launcher.py` & `uranie-launcher-2.0.0/src/uranie_launcher/launcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,72 @@
 """ Script for launching a study with URANIE.
-    It reads study parameters from uncertainty_data subclasses,
+    It reads study parameters from input_data subclasses,
     and runs the script (or the command) commands_to_execute,
     which executes the individual calculation as many times as required.
 """
 
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Tuple
 from uranie_launcher import _data_2_uranie as d2u
-from uranie_launcher import uncertainty_data, execution as exe
-
-from uranie_launcher._data_2_uranie import (STUDY_EXP_DESIGN,   # pylint: disable=unused-import
-                                            STUDY_WORKDIR_NAME,
-                                            STUDY_OUTFILE_NAME,
-                                            STUDY_OUTFILE_NAME_FAILED)
+from uranie_launcher import input_data, execution as exe
 
 
 def execute_uranie(commands_to_execute: Dict[str, List],
-                   inputs: uncertainty_data.Inputs,
-                   propagation: uncertainty_data.Propagation,
-                   outputs: uncertainty_data.Outputs,
+                   inputs: input_data.Inputs,
+                   propagation: input_data.Propagation,
+                   outputs: input_data.Outputs,
                    execution: exe.Execution,
-                   output_dirname: Path,
-                   unitary_result_filename: str) -> int:
+                   output_directory: Path) -> Tuple[Path, int]:
     """ Use URANIE to genetrate the experiment plan based on inputs, then launch calculations.
 
     Parameters
     ----------
     commands_to_execute: Dict[str, List]
         Name of the script or the command which URANIE will execute with all its arguments.
-    inputs: uncertainty_data.Inputs
+    inputs: input_data.Inputs
         Object containing all the infos about the uncertain parameters.
-    propagation: uncertainty_data.Propagation
+    propagation: input_data.Propagation
         Object containing the name of the propagation method used.
-    outputs: uncertainty_data.Outputs
+    outputs: input_data.Outputs
         Object containing the name of the outputs and all the informations about them.
     execution: execution.Execution
         Object containing all the infos about how to execute the calculations.
-    output_dirname: Path
+    output_directory: Path
         Name of the directory where are stored the results
         of the uncertainty quantification calculation
-    unitary_result_filename: str
-        Name of the file containing the result of the
-        aggregations functions for an unitary calculation
 
     Returns
     -------
-    _rootlogon.DataServer.TDataServer
-        return t_data_server if this function run through its end without crashing.
+    Path
+        Path to output file defined as ``output_directory/outputs.output_filename``.
     """
 
     t_data_server = d2u.create_data_server(outputs)
 
     d2u.set_inputs(inputs, t_data_server)
 
-    d2u.generate_sample(propagation, t_data_server, output_dirname)
+    d2u.generate_sample(propagation, outputs, t_data_server, output_directory)
 
-    if execution.visualization:
+    if execution.visualization:  # pragma: no cover
         d2u.visualisation(t_data_server)
 
-    t_output_file, headers = d2u.set_outputs(outputs, unitary_result_filename)
+    t_output_files = d2u.set_outputs(outputs)
 
     # Code instantiation
-    t_launcher, uranie_work_dir = d2u.create_launcher(commands_to_execute,
+    t_launcher = d2u.create_launcher(commands_to_execute,
                                      t_data_server,
-                                     output_dirname,
-                                     t_output_file)
+                                     output_directory,
+                                     t_output_files)
 
-    d2u.run_calculations(execution, t_launcher)
+    d2u.run_calculations(execution, t_launcher, output_directory)
 
-    d2u.save_calculations(propagation,
-                          t_data_server,
-                          headers,
-                          output_dirname,
-                          unitary_result_filename,
-                          uranie_work_dir)
+    ascii_filepath, nb_failed = d2u.save_calculations(propagation,
+                                                      execution,
+                                                      outputs,
+                                                      t_data_server,
+                                                      output_directory)
 
-    if execution.visualization:
+    if execution.visualization:  # pragma: no cover
+        d2u.visualisation(t_data_server)
         input('Type Enter to quit the program...')
 
-    return t_data_server
+    return ascii_filepath, nb_failed
```

### Comparing `uranie-launcher-1.0.1/src/uranie_launcher/uncertainty_data.py` & `uranie-launcher-2.0.0/src/uranie_launcher/input_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-""" Class used to set uncertainty data into an understandable format for uranie_launcher.
+""" Module used to set uncertainty data into an understandable format for uranie_launcher.
 """
 from pathlib import Path
 from typing import List
 
+
 class Inputs():
     """ Class containing all the info about all the uncertain parameters.
     """
-    class Distribution():
+    class Distribution():  # pylint: disable=too-few-public-methods
         """ Class containing the info about the distribution for a specific uncertain parameter.
         """
         def __init__(self):
             pass
 
         # TODO string conversion
         # def __str__(self) -> str:
@@ -31,26 +32,26 @@
             if lower_bound < upper_bound:
                 self._lower_bound = lower_bound
                 self._upper_bound = upper_bound
             else:
                 raise ValueError("The upper bound have to be greater than the lower one !")
 
         @property
-        def lower_bound(self):
+        def lower_bound(self) -> float:
             """Returns info about the distribution
 
             Returns
             -------
             float
                 lower bound of the distribution
             """
             return self._lower_bound
 
         @property
-        def upper_bound(self):
+        def upper_bound(self) -> float:
             """Returns info about the distribution
 
             Returns
             -------
             float
                 upper bound of the distribution
             """
@@ -77,48 +78,48 @@
                 self._upper_bound = upper_bound
                 self._mean = mean
                 self._standard_deviation = standard_deviation
             else:
                 raise ValueError("The upper bound have to be greater than the lower one !")
 
         @property
-        def lower_bound(self):
+        def lower_bound(self) -> float:
             """Returns all info about the distribution
 
             Returns
             -------
             float
                 lower bound of the distribution
             """
             return self._lower_bound
 
         @property
-        def upper_bound(self):
+        def upper_bound(self) -> float:
             """Returns all info about the distribution
 
             Returns
             -------
             float
                 upper bound of the distribution
             """
             return self._upper_bound
 
         @property
-        def mean(self):
+        def mean(self) -> float:
             """Returns all info about the distribution
 
             Returns
             -------
             float
                 mean
             """
             return self._mean
 
         @property
-        def standard_deviation(self):
+        def standard_deviation(self) -> float:
             """Returns all info about the distribution
 
             Returns
             -------
             float
                 standard deviation
             """
@@ -138,37 +139,37 @@
                 Is the distribution_info object previously defined
             """
             self._variable_name = variable_name
             self._distribution = distribution
             self._flag_delimiter = '@'
 
         @property
-        def variable_name(self):
+        def variable_name(self) -> str:
             """Returns the name of the uncertain value
 
             Returns
             -------
             str
                 variable name
             """
             return self._variable_name
 
         @property
-        def distribution(self):
+        def distribution(self) -> 'Inputs.Distribution':
             """Returns all info about the distribution
 
             Returns
             -------
-            list
+            'Inputs.Distribution'
                 distribution
             """
             return self._distribution
 
         @property
-        def flag(self):
+        def flag(self) -> str:
             """Returns the flag
 
             Returns
             -------
             str
                 flag
             """
@@ -186,15 +187,15 @@
         ----------
         _input : Input
             Object containing all the info about one specific parameter of the uncertain parameters.
         """
         self._inputs.append(_input)
 
     @property
-    def inputs(self):
+    def inputs(self) -> List[Input]:
         """Returns the _inputs list that contains all info about each uncertain parameter
 
         Returns
         -------
         list
             inputs
         """
@@ -208,15 +209,15 @@
         ----------
         file_flag : Path
             Should be something like : <file_name>_Balise.<ext>
         """
         self._file_flag = file_flag
 
     @property
-    def file_flag(self):
+    def file_flag(self) -> str:
         """Returns the name of the file containing the balise
 
         Returns
         -------
         str
             file flag
         """
@@ -238,80 +239,95 @@
         if sample_size <= 0:
             raise ValueError("sample_size must be greater than 0")
 
         self._sampling_method = sampling_method
         self._sample_size = sample_size
 
     @property
-    def sampling_method(self):
+    def sampling_method(self) -> str:
         """Returns the sampling method
 
         Returns
         -------
         str
             sampling method name
         """
         return self._sampling_method
 
     @property
-    def sample_size(self):
+    def sample_size(self) -> int:
         """Get the sample size variable
 
         Returns
         -------
         int
             sample size
         """
         return self._sample_size
 
 
 class Outputs():
     """ Class defining an object containing all the informations about the outputs.
     """
+
     class Output():
         """ Class containing all the info about one specific output.
         """
-        def __init__(self, headers: List[str], quantity_of_interest: str):
+        def __init__(self, headers: List[str], quantity_of_interest: str, filename: str):
             """Constructor.
 
             Parameters
             ----------
             headers : List[str]
                 Names of the aggregation functions applied on the output
             quantity_of_interest : str
                 Names of the output
+            filename : str
+                Name of the output file, if any
             """
             self._headers = headers
             self._quantity_of_interest = quantity_of_interest
+            self._filename = filename
 
         @property
-        def headers(self):
+        def headers(self) -> List[str]:
             """Returns the dictionary containing all the chosen aggregation functions
 
             Returns
             -------
             list
                 headers
             """
             return self._headers
 
         @property
-        def quantity_of_interest(self):
+        def quantity_of_interest(self) -> str:
             """Returns the name of the quantity of interest
 
             Returns
             -------
-            list
+            str
                 quantity_of_interest
             """
             return self._quantity_of_interest
 
-    def __init__(self, tds_name):
+        @property
+        def filename(self) -> str:
+            """Returns the name of the output file, if any
+
+            Returns
+            -------
+            str
+                file name
+            """
+            return self._filename
+
+    def __init__(self, name):
         self._outputs = []
-        self._tds_name = tds_name
+        self._name = name
 
     def add_output(self, output: 'Outputs.Output'):
         """ Set all the info about one specific output.
 
         Parameters
         ----------
         output : Outputs.Output
@@ -327,16 +343,49 @@
         -------
         List[Output]
             outputs
         """
         return self._outputs
 
     @property
-    def name(self):
-        """Returns the name of the output (bof, pas sur...)
+    def name(self) -> str:
+        """Returns the name of the output
 
         Returns
         -------
-        list
+        str
             tds_name
         """
-        return self._tds_name
+        return self._name
+
+    @property
+    def experimental_design_filename(self) -> str:
+        """Returns the name of the experimental design file
+
+        Returns
+        -------
+        str
+            ``self.name+'_exp_design.dat')``
+        """
+        return f"{self.name}_exp_design.dat"
+
+    @property
+    def output_filename(self) -> str:
+        """Returns the name of the output file
+
+        Returns
+        -------
+        str
+            ``self.name+'_output.dat')``
+        """
+        return f"{self.name}_output.dat"
+
+    @property
+    def failed_filename(self) -> str:
+        """Returns the name of the failed file
+
+        Returns
+        -------
+        str
+            ``self.name+'_failed.dat')``
+        """
+        return f"{self.name}_failed.dat"
```

### Comparing `uranie-launcher-1.0.1/src/uranie_launcher/utils.py` & `uranie-launcher-2.0.0/src/uranie_launcher/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 """Define the different verbosity of the logs.
 """
 
-_log_level = 1
+_log_level = 1  # pylint: disable=invalid-name
+"""Verbosity level"""
 
 NONE = 0
 INFO = 1
 DEBUG = 2
 
+
 def set_verbosity(log_level: int):
     """Define verbosity level.
 
     Parameters
     ----------
     log_level : int
         log level
 
     Raises
     ------
     ValueError
         if not in range [NONE;DEBUG]
     """
-    global _log_level
-    if not (NONE <= log_level <= DEBUG):
+    global _log_level  # pylint: disable=invalid-name,global-statement
+    if not NONE <= log_level <= DEBUG:
         raise ValueError(f"log_level must be in [{NONE};{DEBUG}]")
     _log_level = log_level
 
+
+def get_log_level():
+    """Access to current log level."""
+    return _log_level
+
+
 def log(level, *args, **kwargs):
     """log basis function"""
+    if level >= DEBUG and "flush" not in kwargs:
+        kwargs["flush"] = True
     if _log_level >= level:
         print(*args, **kwargs)
 
+
 def info(*args, **kwargs):
     """Log info level. Use it as print function."""
     log(INFO, *args, **kwargs)
 
+
 def debug(*args, **kwargs):
     """Log debug level. Use it as print function."""
     log(DEBUG, *args, **kwargs)
```

### Comparing `uranie-launcher-1.0.1/src/uranie_launcher.egg-info/PKG-INFO` & `uranie-launcher-2.0.0/src/uranie_launcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uranie-launcher
-Version: 1.0.1
+Version: 2.0.0
 Summary: uranie-launcher help you to run your calculation scripts with Uranie
 Home-page: UNKNOWN
 Author: Clément STUTZ
 Author-email: clement.stutz@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/clementstutz/uranie-launcher/issues
 Project-URL: Source, https://github.com/clementstutz/uranie-launcher
```

### Comparing `uranie-launcher-1.0.1/src/uranie_launcher.egg-info/SOURCES.txt` & `uranie-launcher-2.0.0/src/uranie_launcher.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/uranie_launcher/VERSION
 src/uranie_launcher/__init__.py
 src/uranie_launcher/_data_2_uranie.py
-src/uranie_launcher/_rootlogon.py
 src/uranie_launcher/_run_unitary.py
+src/uranie_launcher/data.py
 src/uranie_launcher/execution.py
+src/uranie_launcher/input_data.py
 src/uranie_launcher/launcher.py
-src/uranie_launcher/uncertainty_data.py
 src/uranie_launcher/utils.py
 src/uranie_launcher.egg-info/PKG-INFO
 src/uranie_launcher.egg-info/SOURCES.txt
 src/uranie_launcher.egg-info/dependency_links.txt
 src/uranie_launcher.egg-info/entry_points.txt
 src/uranie_launcher.egg-info/requires.txt
 src/uranie_launcher.egg-info/top_level.txt
```

### Comparing `uranie-launcher-1.0.1/LICENSE` & `uranie-launcher-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uranie-launcher-1.0.1/README.md` & `uranie-launcher-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `uranie-launcher-1.0.1/setup.py` & `uranie-launcher-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `uranie-launcher-1.0.1/PKG-INFO` & `uranie-launcher-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uranie-launcher
-Version: 1.0.1
+Version: 2.0.0
 Summary: uranie-launcher help you to run your calculation scripts with Uranie
 Home-page: UNKNOWN
 Author: Clément STUTZ
 Author-email: clement.stutz@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/clementstutz/uranie-launcher/issues
 Project-URL: Source, https://github.com/clementstutz/uranie-launcher
```

