# Comparing `tmp/pyvrp-0.4.4.tar.gz` & `tmp/pyvrp-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvrp-0.4.4.tar", max compression
+gzip compressed data, was "pyvrp-0.5.0.tar", max compression
```

## Comparing `pyvrp-0.4.4.tar` & `pyvrp-0.5.0.tar`

### file list

```diff
@@ -1,149 +1,146 @@
--rw-r--r--   0        0        0     1175 2023-07-09 13:25:12.450763 pyvrp-0.4.4/LICENSE.md
--rw-r--r--   0        0        0     2963 2023-07-09 13:25:12.450763 pyvrp-0.4.4/README.md
--rw-r--r--   0        0        0     3563 2023-07-09 13:25:12.450763 pyvrp-0.4.4/build_extensions.py
--rw-r--r--   0        0        0     3155 2023-07-09 13:25:12.478762 pyvrp-0.4.4/meson.build
--rw-r--r--   0        0        0      302 2023-07-09 13:25:12.478762 pyvrp-0.4.4/meson_options.txt
--rw-r--r--   0        0        0     3456 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     6848 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/GeneticAlgorithm.py
--rw-r--r--   0        0        0     8536 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/Model.py
--rw-r--r--   0        0        0     8799 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/PenaltyManager.py
--rw-r--r--   0        0        0     6551 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/Population.py
--rw-r--r--   0        0        0     2892 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/Result.py
--rw-r--r--   0        0        0     6183 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/Statistics.py
--rw-r--r--   0        0        0      510 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/__init__.py
--rw-r--r--   0        0        0    20429 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/_pyvrp.pyi
--rw-r--r--   0        0        0     9113 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cli.py
--rw-r--r--   0        0        0       45 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/constants.py
--rw-r--r--   0        0        0      925 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/CostEvaluator.cpp
--rw-r--r--   0        0        0     2079 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/CostEvaluator.h
--rw-r--r--   0        0        0     2178 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/DynamicBitset.cpp
--rw-r--r--   0        0        0     1618 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/DynamicBitset.h
--rw-r--r--   0        0        0     2791 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/Matrix.h
--rw-r--r--   0        0        0     5732 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/Measure.h
--rw-r--r--   0        0        0     2701 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/ProblemData.cpp
--rw-r--r--   0        0        0     4778 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/ProblemData.h
--rw-r--r--   0        0        0      871 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/README.md
--rw-r--r--   0        0        0    11122 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/Solution.cpp
--rw-r--r--   0        0        0     6990 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/Solution.h
--rw-r--r--   0        0        0     4709 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/SubPopulation.cpp
--rw-r--r--   0        0        0     3116 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/SubPopulation.h
--rw-r--r--   0        0        0     3765 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/TimeWindowSegment.h
--rw-r--r--   0        0        0      608 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/XorShift128.cpp
--rw-r--r--   0        0        0     2149 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/XorShift128.h
--rw-r--r--   0        0        0    19239 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/bindings.cpp
--rw-r--r--   0        0        0      378 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/crossover/bindings.cpp
--rw-r--r--   0        0        0     5508 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/crossover/crossover.cpp
--rw-r--r--   0        0        0     2048 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/crossover/crossover.h
--rw-r--r--   0        0        0     8327 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/crossover/selective_route_exchange.cpp
--rw-r--r--   0        0        0      260 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/diversity/bindings.cpp
--rw-r--r--   0        0        0     1080 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/diversity/broken_pairs_distance.cpp
--rw-r--r--   0        0        0      698 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/diversity/diversity.h
--rw-r--r--   0        0        0     3104 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/CircleSector.h
--rw-r--r--   0        0        0    11481 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/Exchange.h
--rw-r--r--   0        0        0    14616 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/LocalSearch.cpp
--rw-r--r--   0        0        0     3790 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/LocalSearch.h
--rw-r--r--   0        0        0     2703 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/LocalSearchOperator.h
--rw-r--r--   0        0        0     3728 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/MoveTwoClientsReversed.cpp
--rw-r--r--   0        0        0      560 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/MoveTwoClientsReversed.h
--rw-r--r--   0        0        0      998 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/Node.cpp
--rw-r--r--   0        0        0     1672 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/Node.h
--rw-r--r--   0        0        0     1267 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/RelocateStar.cpp
--rw-r--r--   0        0        0      811 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/RelocateStar.h
--rw-r--r--   0        0        0     4002 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/Route.cpp
--rw-r--r--   0        0        0     5421 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/Route.h
--rw-r--r--   0        0        0    11059 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/SwapStar.cpp
--rw-r--r--   0        0        0     3455 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/SwapStar.h
--rw-r--r--   0        0        0     4407 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/TwoOpt.cpp
--rw-r--r--   0        0        0      978 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/TwoOpt.h
--rw-r--r--   0        0        0     4633 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/bindings.cpp
--rw-r--r--   0        0        0       63 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/crossover/__init__.py
--rw-r--r--   0        0        0      292 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/crossover/_crossover.pyi
--rw-r--r--   0        0        0     1826 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/crossover/selective_route_exchange.py
--rw-r--r--   0        0        0    13200 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/crossover/tests/test_selective_route_exchange.py
--rw-r--r--   0        0        0       46 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/diversity/__init__.py
--rw-r--r--   0        0        0     1441 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/diversity/_diversity.pyi
--rw-r--r--   0        0        0     1171 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/diversity/tests/test_broken_pairs_distance.py
--rw-r--r--   0        0        0      580 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/exceptions.py
--rw-r--r--   0        0        0      436 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/__init__.py
--rw-r--r--   0        0        0     1106 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_coordinates.py
--rw-r--r--   0        0        0     1358 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_demands.py
--rw-r--r--   0        0        0     1199 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_diversity.py
--rw-r--r--   0        0        0     1129 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_instance.py
--rw-r--r--   0        0        0     2344 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_objectives.py
--rw-r--r--   0        0        0     1608 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_result.py
--rw-r--r--   0        0        0     4690 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_route_schedule.py
--rw-r--r--   0        0        0     1136 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_runtimes.py
--rw-r--r--   0        0        0     1782 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/plot_solution.py
--rw-r--r--   0        0        0     1226 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/plot_time_windows.py
--rw-r--r--   0        0        0        0 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/__init__.py
--rw-r--r--   0        0        0    47981 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png
--rw-r--r--   0        0        0   141297 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png
--rw-r--r--   0        0        0    35194 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png
--rw-r--r--   0        0        0    25609 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png
--rw-r--r--   0        0        0    43058 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png
--rw-r--r--   0        0        0     3079 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/test_plotting.py
--rw-r--r--   0        0        0     6776 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/read.py
--rw-r--r--   0        0        0     6515 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/LocalSearch.py
--rw-r--r--   0        0        0      643 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/__init__.py
--rw-r--r--   0        0        0     2113 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/_search.pyi
--rw-r--r--   0        0        0     5105 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/neighbourhood.py
--rw-r--r--   0        0        0        0 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/__init__.py
--rw-r--r--   0        0        0    10448 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_Exchange.py
--rw-r--r--   0        0        0     8605 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_LocalSearch.py
--rw-r--r--   0        0        0     2633 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_MoveTwoClientsReversed.py
--rw-r--r--   0        0        0     3029 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_RelocateStar.py
--rw-r--r--   0        0        0     2918 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_SwapStar.py
--rw-r--r--   0        0        0     3970 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_TwoOpt.py
--rw-r--r--   0        0        0     6091 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_neighbourhood.py
--rw-r--r--   0        0        0     1048 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/show_versions.py
--rw-r--r--   0        0        0      444 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/MaxIterations.py
--rw-r--r--   0        0        0      589 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/MaxRuntime.py
--rw-r--r--   0        0        0      819 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/NoImprovement.py
--rw-r--r--   0        0        0      573 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/StoppingCriterion.py
--rw-r--r--   0        0        0      575 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/TimedNoImprovement.py
--rw-r--r--   0        0        0      217 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/tests/__init__.py
--rw-r--r--   0        0        0      839 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/tests/test_MaxIterations.py
--rw-r--r--   0        0        0     1031 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/tests/test_MaxRuntime.py
--rw-r--r--   0        0        0     1777 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/tests/test_NoImprovement.py
--rw-r--r--   0        0        0     1292 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/tests/test_TimedNoImprovement.py
--rw-r--r--   0        0        0        0 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/__init__.py
--rw-r--r--   0        0        0      189 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/DepotNotOne.txt
--rw-r--r--   0        0        0      607 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/E-n22-k4.txt
--rw-r--r--   0        0        0      671 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/EdgeWeightsNoExplicit.txt
--rw-r--r--   0        0        0      668 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt
--rw-r--r--   0        0        0      389 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/FileWithUnknownSection.txt
--rw-r--r--   0        0        0      191 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/MoreThanOneDepot.txt
--rw-r--r--   0        0        0      371 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/NonZeroDepotDemand.txt
--rw-r--r--   0        0        0      371 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/NonZeroDepotOpenTimeWindow.txt
--rw-r--r--   0        0        0      371 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/NonZeroDepotReleaseTime.txt
--rw-r--r--   0        0        0      371 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/NonZeroDepotServiceDuration.txt
--rw-r--r--   0        0        0      675 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/OkSmall.txt
--rw-r--r--   0        0        0      697 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/OkSmallGreedyRepair.txt
--rw-r--r--   0        0        0      754 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/OkSmallPrizes.txt
--rw-r--r--   0        0        0      744 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/OkSmallReleaseTimes.txt
--rw-r--r--   0        0        0      347 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/RC208.sol
--rw-r--r--   0        0        0     7524 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/RC208.txt
--rw-r--r--   0        0        0      681 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/ReallyLargeDistance.txt
--rw-r--r--   0        0        0      369 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/TimeWindowOpenLargerThanClose.txt
--rw-r--r--   0        0        0      187 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/UnknownEdgeWeightFmt.txt
--rw-r--r--   0        0        0      154 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/UnknownEdgeWeightType.txt
--rw-r--r--   0        0        0     2005 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/p06-2-50.vrp
--rw-r--r--   0        0        0     1985 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/helpers.py
--rw-r--r--   0        0        0     4674 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/test_CostEvaluator.py
--rw-r--r--   0        0        0     2869 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/test_DynamicBitset.py
--rw-r--r--   0        0        0     7717 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_GeneticAlgorithm.py
--rw-r--r--   0        0        0     1347 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Matrix.py
--rw-r--r--   0        0        0     8491 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Model.py
--rw-r--r--   0        0        0     9864 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_PenaltyManager.py
--rw-r--r--   0        0        0    12503 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Population.py
--rw-r--r--   0        0        0     3570 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_ProblemData.py
--rw-r--r--   0        0        0     2645 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Result.py
--rw-r--r--   0        0        0    19074 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Solution.py
--rw-r--r--   0        0        0     1134 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Statistics.py
--rw-r--r--   0        0        0     5874 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_SubPopulation.py
--rw-r--r--   0        0        0     2203 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_TimeWindowSegment.py
--rw-r--r--   0        0        0     1088 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_XorShift128.py
--rw-r--r--   0        0        0     7153 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_read.py
--rw-r--r--   0        0        0      616 2023-07-09 13:25:12.486762 pyvrp-0.4.4/subprojects/pybind11.wrap
--rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pyvrp-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1172 2023-08-02 08:47:21.187546 pyvrp-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     3326 2023-08-02 08:47:21.187546 pyvrp-0.5.0/README.md
+-rw-r--r--   0        0        0     3565 2023-08-02 08:47:21.187546 pyvrp-0.5.0/build_extensions.py
+-rw-r--r--   0        0        0     3982 2023-08-02 08:47:21.187546 pyvrp-0.5.0/meson.build
+-rw-r--r--   0        0        0      302 2023-08-02 08:47:21.187546 pyvrp-0.5.0/meson_options.txt
+-rw-r--r--   0        0        0     3754 2023-08-02 08:47:21.187546 pyvrp-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6458 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/GeneticAlgorithm.py
+-rw-r--r--   0        0        0     8554 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/Model.py
+-rw-r--r--   0        0        0     8718 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/PenaltyManager.py
+-rw-r--r--   0        0        0     6648 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/Population.py
+-rw-r--r--   0        0        0     2232 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/Result.py
+-rw-r--r--   0        0        0     6199 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/Statistics.py
+-rw-r--r--   0        0        0      520 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/__init__.py
+-rw-r--r--   0        0        0     6903 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/_pyvrp.pyi
+-rw-r--r--   0        0        0     8798 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cli.py
+-rw-r--r--   0        0        0       45 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/constants.py
+-rw-r--r--   0        0        0      226 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/CostEvaluator.cpp
+-rw-r--r--   0        0        0     4227 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/CostEvaluator.h
+-rw-r--r--   0        0        0     2178 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/DynamicBitset.cpp
+-rw-r--r--   0        0        0     1618 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/DynamicBitset.h
+-rw-r--r--   0        0        0     2791 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/Matrix.h
+-rw-r--r--   0        0        0     5686 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/Measure.h
+-rw-r--r--   0        0        0     3101 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/ProblemData.cpp
+-rw-r--r--   0        0        0     8660 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/ProblemData.h
+-rw-r--r--   0        0        0     1138 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/README.md
+-rw-r--r--   0        0        0      668 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/RandomNumberGenerator.cpp
+-rw-r--r--   0        0        0     2237 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/RandomNumberGenerator.h
+-rw-r--r--   0        0        0    11018 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/Solution.cpp
+-rw-r--r--   0        0        0    12632 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/Solution.h
+-rw-r--r--   0        0        0     4709 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/SubPopulation.cpp
+-rw-r--r--   0        0        0     4805 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/SubPopulation.h
+-rw-r--r--   0        0        0      690 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/TimeWindowSegment.cpp
+-rw-r--r--   0        0        0     5709 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/TimeWindowSegment.h
+-rw-r--r--   0        0        0    25587 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/bindings.cpp
+-rw-r--r--   0        0        0      463 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/crossover/bindings.cpp
+-rw-r--r--   0        0        0     5501 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/crossover/crossover.cpp
+-rw-r--r--   0        0        0     1839 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/crossover/crossover.h
+-rw-r--r--   0        0        0     8023 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/crossover/selective_route_exchange.cpp
+-rw-r--r--   0        0        0      342 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/diversity/bindings.cpp
+-rw-r--r--   0        0        0     1080 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/diversity/broken_pairs_distance.cpp
+-rw-r--r--   0        0        0     1682 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/diversity/diversity.h
+-rw-r--r--   0        0        0    12272 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/Exchange.h
+-rw-r--r--   0        0        0    14775 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/LocalSearch.cpp
+-rw-r--r--   0        0        0     4286 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/LocalSearch.h
+-rw-r--r--   0        0        0     2710 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/LocalSearchOperator.h
+-rw-r--r--   0        0        0     3756 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/MoveTwoClientsReversed.cpp
+-rw-r--r--   0        0        0      627 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/MoveTwoClientsReversed.h
+-rw-r--r--   0        0        0     1205 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/RelocateStar.cpp
+-rw-r--r--   0        0        0      825 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/RelocateStar.h
+-rw-r--r--   0        0        0     4085 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/Route.cpp
+-rw-r--r--   0        0        0     7717 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/Route.h
+-rw-r--r--   0        0        0    11203 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/SwapStar.cpp
+-rw-r--r--   0        0        0     3668 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/SwapStar.h
+-rw-r--r--   0        0        0     4829 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/TwoOpt.cpp
+-rw-r--r--   0        0        0     1147 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/TwoOpt.h
+-rw-r--r--   0        0        0     5371 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/cpp/search/bindings.cpp
+-rw-r--r--   0        0        0       63 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/crossover/__init__.py
+-rw-r--r--   0        0        0      292 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/crossover/_crossover.pyi
+-rw-r--r--   0        0        0     1867 2023-08-02 08:47:21.191546 pyvrp-0.5.0/pyvrp/crossover/selective_route_exchange.py
+-rw-r--r--   0        0        0    13261 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/crossover/tests/test_selective_route_exchange.py
+-rw-r--r--   0        0        0       46 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/diversity/__init__.py
+-rw-r--r--   0        0        0      110 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/diversity/_diversity.pyi
+-rw-r--r--   0        0        0     1171 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/diversity/tests/test_broken_pairs_distance.py
+-rw-r--r--   0        0        0      382 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/exceptions.py
+-rw-r--r--   0        0        0      436 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/__init__.py
+-rw-r--r--   0        0        0     1106 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/plot_coordinates.py
+-rw-r--r--   0        0        0     1358 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/plot_demands.py
+-rw-r--r--   0        0        0      891 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/plot_diversity.py
+-rw-r--r--   0        0        0     1129 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/plot_instance.py
+-rw-r--r--   0        0        0     2036 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/plot_objectives.py
+-rw-r--r--   0        0        0     1545 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/plot_result.py
+-rw-r--r--   0        0        0     4684 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/plot_route_schedule.py
+-rw-r--r--   0        0        0      820 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/plot_runtimes.py
+-rw-r--r--   0        0        0     1772 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/plot_solution.py
+-rw-r--r--   0        0        0     1226 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/plot_time_windows.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/tests/__init__.py
+-rw-r--r--   0        0        0    47981 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png
+-rw-r--r--   0        0        0   141297 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png
+-rw-r--r--   0        0        0    35194 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png
+-rw-r--r--   0        0        0    25609 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png
+-rw-r--r--   0        0        0    43058 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png
+-rw-r--r--   0        0        0     2280 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/plotting/tests/test_plotting.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/py.typed
+-rw-r--r--   0        0        0     6518 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/read.py
+-rw-r--r--   0        0        0     5182 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/search/LocalSearch.py
+-rw-r--r--   0        0        0      699 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/search/SearchMethod.py
+-rw-r--r--   0        0        0      682 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/search/__init__.py
+-rw-r--r--   0        0        0     2273 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/search/_search.pyi
+-rw-r--r--   0        0        0     5198 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/search/neighbourhood.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/search/tests/__init__.py
+-rw-r--r--   0        0        0    10549 2023-08-02 08:47:21.195546 pyvrp-0.5.0/pyvrp/search/tests/test_Exchange.py
+-rw-r--r--   0        0        0    13657 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/search/tests/test_LocalSearch.py
+-rw-r--r--   0        0        0     2663 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/search/tests/test_MoveTwoClientsReversed.py
+-rw-r--r--   0        0        0     3039 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/search/tests/test_RelocateStar.py
+-rw-r--r--   0        0        0     2914 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/search/tests/test_SwapStar.py
+-rw-r--r--   0        0        0     4035 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/search/tests/test_TwoOpt.py
+-rw-r--r--   0        0        0     6198 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/search/tests/test_neighbourhood.py
+-rw-r--r--   0        0        0     1048 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/show_versions.py
+-rw-r--r--   0        0        0      444 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/stop/MaxIterations.py
+-rw-r--r--   0        0        0      589 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/stop/MaxRuntime.py
+-rw-r--r--   0        0        0      819 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/stop/NoImprovement.py
+-rw-r--r--   0        0        0      561 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/stop/StoppingCriterion.py
+-rw-r--r--   0        0        0      575 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/stop/TimedNoImprovement.py
+-rw-r--r--   0        0        0      217 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/stop/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/stop/tests/__init__.py
+-rw-r--r--   0        0        0      839 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/stop/tests/test_MaxIterations.py
+-rw-r--r--   0        0        0     1031 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/stop/tests/test_MaxRuntime.py
+-rw-r--r--   0        0        0     1781 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/stop/tests/test_NoImprovement.py
+-rw-r--r--   0        0        0     1300 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/stop/tests/test_TimedNoImprovement.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/__init__.py
+-rw-r--r--   0        0        0      189 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/DepotNotOne.txt
+-rw-r--r--   0        0        0      607 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/E-n22-k4.txt
+-rw-r--r--   0        0        0      671 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/EdgeWeightsNoExplicit.txt
+-rw-r--r--   0        0        0      668 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt
+-rw-r--r--   0        0        0      389 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/FileWithUnknownSection.txt
+-rw-r--r--   0        0        0      191 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/MoreThanOneDepot.txt
+-rw-r--r--   0        0        0      675 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/OkSmall.txt
+-rw-r--r--   0        0        0      697 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/OkSmallGreedyRepair.txt
+-rw-r--r--   0        0        0      754 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/OkSmallPrizes.txt
+-rw-r--r--   0        0        0      744 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/OkSmallReleaseTimes.txt
+-rw-r--r--   0        0        0      701 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/OkSmallWaitTime.txt
+-rw-r--r--   0        0        0      347 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/RC208.sol
+-rw-r--r--   0        0        0     7524 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/RC208.txt
+-rw-r--r--   0        0        0      681 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/ReallyLargeDistance.txt
+-rw-r--r--   0        0        0      369 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/TimeWindowOpenLargerThanClose.txt
+-rw-r--r--   0        0        0      187 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/UnknownEdgeWeightFmt.txt
+-rw-r--r--   0        0        0      154 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/UnknownEdgeWeightType.txt
+-rw-r--r--   0        0        0     2005 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/data/p06-2-50.vrp
+-rw-r--r--   0        0        0     1985 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/helpers.py
+-rw-r--r--   0        0        0     4674 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_CostEvaluator.py
+-rw-r--r--   0        0        0     2873 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_DynamicBitset.py
+-rw-r--r--   0        0        0     6186 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_GeneticAlgorithm.py
+-rw-r--r--   0        0        0     1347 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_Matrix.py
+-rw-r--r--   0        0        0     9382 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_Model.py
+-rw-r--r--   0        0        0     9905 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_PenaltyManager.py
+-rw-r--r--   0        0        0    12682 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_Population.py
+-rw-r--r--   0        0        0     5402 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_ProblemData.py
+-rw-r--r--   0        0        0     1158 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_RandomNumberGenerator.py
+-rw-r--r--   0        0        0     2551 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_Result.py
+-rw-r--r--   0        0        0    23989 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_Solution.py
+-rw-r--r--   0        0        0     1154 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_Statistics.py
+-rw-r--r--   0        0        0     5935 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_SubPopulation.py
+-rw-r--r--   0        0        0     2203 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_TimeWindowSegment.py
+-rw-r--r--   0        0        0     6934 2023-08-02 08:47:21.199546 pyvrp-0.5.0/pyvrp/tests/test_read.py
+-rw-r--r--   0        0        0      616 2023-08-02 08:47:21.199546 pyvrp-0.5.0/subprojects/pybind11.wrap
+-rw-r--r--   0        0        0     4451 1970-01-01 00:00:00.000000 pyvrp-0.5.0/PKG-INFO
```

### Comparing `pyvrp-0.4.4/LICENSE.md` & `pyvrp-0.5.0/LICENSE.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 MIT License
 
-Copyright (c) 2020, Thibaut Vidal (HGS-CVRP)
-Copyright (c) 2022, ORTEC and TU/e (HGS-DIMACS)
-Copyright (c) since 2022, PyVRP contributors
+- Copyright (c) 2020, Thibaut Vidal (HGS-CVRP)
+- Copyright (c) 2022, ORTEC (HGS-DIMACS)
+- Copyright (c) since 2022, PyVRP contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyvrp-0.4.4/README.md` & `pyvrp-0.5.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-![PyVRP logo](docs/source/assets/images/PyVRP.svg)
+![PyVRP logo](docs/source/assets/images/logo.svg)
 
 [![PyPI version](https://badge.fury.io/py/pyvrp.svg)](https://badge.fury.io/py/pyvrp)
 [![CI](https://github.com/PyVRP/PyVRP/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/PyVRP/PyVRP/actions/workflows/CI.yml)
-[![Documentation Status](https://readthedocs.org/projects/pyvrp/badge/?version=latest)](https://pyvrp.readthedocs.io/en/latest/?badge=latest)
+[![DOC](https://github.com/PyVRP/PyVRP/actions/workflows/DOC.yml/badge.svg?branch=main)](https://pyvrp.org/)
 [![codecov](https://codecov.io/gh/PyVRP/PyVRP/branch/main/graph/badge.svg?token=G9JKIVZOHB)](https://codecov.io/gh/PyVRP/PyVRP)
 
-The `pyvrp` package is an open-source, state-of-the-art vehicle routing problem (VRP) solver.
-It currently supports the capacitated VRP (CVRP), the VRP with time windows (VRPTW), and prize-collecting. 
+PyVRP is an open-source, state-of-the-art vehicle routing problem (VRP) solver.
+It currently supports VRPs with:
+- Client demands (capacitated VRP);
+- Vehicles of different capacities;
+- Time windows, client service durations, and release times (VRP with time windows and release times);
+- Optional clients with prizes for visiting (prize collecting).
 
 The implementation builds on Thibaut Vidal's [HGS-CVRP][8], but has been completely redesigned to be easy to use as a highly customisable Python package, while maintaining speed and state-of-the-art performance.
 Users can customise various aspects of the algorithm using Python, including population management, crossover strategies, granular neighbourhoods and operator selection in the local search.
-Additionally, for advanced use cases such as supporting additional VRP variants, users can build and install `pyvrp` directly from the source code.
+Additionally, for advanced use cases such as supporting additional VRP variants, users can build and install PyVRP directly from the source code.
 
-`pyvrp` may be installed in the usual way as
+PyVRP is available on the Python package index as `pyvrp`.
+It may be installed in the usual way as
 ```
 pip install pyvrp
 ```
-This also resolves the few core dependencies `pyvrp` has.
+This also resolves the few core dependencies PyVRP has.
 The documentation is available [here][1].
 
 > If you are new to vehicle routing or metaheuristics, you might benefit from first reading the [introduction to VRP][6] and [introduction to HGS][7] pages.
 
 ### Examples
 
-We provide some example notebooks that show how the `pyvrp` package may be used to solve vehicle routing problems.
+We provide some example notebooks that show how PyVRP may be used to solve vehicle routing problems.
 These include:
 
-- The vehicle routing problem with time windows (VRPTW), [here][4].
-  We solve several instances from the literature, including a large 1000 customer instance.
-- The capacitated vehicle routing problem (CVRP), [here][5].
-  We solve an instance with 439 customers to near optimality within 30 seconds.
+- A short tutorial and introduction to PyVRP's modelling interface, [here][5].
+  This is a great way to get started with PyVRP.
+- A notebook solving classical VRP variants, [here][4].
+  In this notebook we solve several benchmark instances of the CVRP and VRPTW problems.
+  We also demonstrate how to use the plotting tools available in PyVRP to visualise the instance and statistics collected during the search procedure. 
+- A notebook implementing a `solve` method using PyVRP's components, [here][9].
+  This notebook is a great way to dive deeper into how PyVRP works internally.
 
 ### Contributing
 
 We are very grateful for any contributions you are willing to make. Please have
 a look [here][2] to get started. If you aim to make a large change, it is
 helpful to discuss the change first in a new GitHub issue. Feel free to open
 one!
@@ -43,22 +51,24 @@
 If you are looking for help, please follow the instructions [here][3].
 
 ### How to cite PyVRP
 
 TODO
 
 
-[1]: https://pyvrp.readthedocs.io/en/latest/
+[1]: https://pyvrp.org/
 
-[2]: https://pyvrp.readthedocs.io/en/latest/dev/contributing.html
+[2]: https://pyvrp.org/dev/contributing.html
 
-[3]: https://pyvrp.readthedocs.io/en/latest/setup/getting_help.html
+[3]: https://pyvrp.org/setup/getting_help.html
 
-[4]: https://pyvrp.readthedocs.io/en/latest/examples/vrptw.html
+[4]: https://pyvrp.org/examples/basic_vrps.html
 
-[5]: https://pyvrp.readthedocs.io/en/latest/examples/cvrp.html
+[5]: https://pyvrp.org/examples/quick_tutorial.html
 
-[6]: https://pyvrp.readthedocs.io/en/latest/setup/introduction_to_vrp.html
+[6]: https://pyvrp.org/setup/introduction_to_vrp.html
 
-[7]: https://pyvrp.readthedocs.io/en/latest/setup/introduction_to_hgs.html
+[7]: https://pyvrp.org/setup/introduction_to_hgs.html
 
 [8]: https://github.com/vidalt/HGS-CVRP/
+
+[9]: https://pyvrp.org/examples/using_pyvrp_components.html
```

### Comparing `pyvrp-0.4.4/build_extensions.py` & `pyvrp-0.5.0/build_extensions.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         help="Clean build and installation directories before building.",
     )
     parser.add_argument(
         "--regenerate_type_stubs",
         action="store_true",
         help="""
         Whether to regenerate the MyPy type stubs as well. Default False, since
-        this can overwrite manual improvements and docstrings.
+        this can overwrite manual adjustments to the type stubs.
         """,
     )
     parser.add_argument(
         "--additional",
         nargs=argparse.REMAINDER,
         default=[],
         help="Extra Meson configuration options (passed verbatim to Meson).",
```

### Comparing `pyvrp-0.4.4/meson.build` & `pyvrp-0.5.0/meson.build`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 project(
     'pyvrp',
     'cpp',
-    version: run_command('poetry', 'version', '--short', check : true).stdout(),
-    default_options : [
+    version: run_command('poetry', 'version', '--short', check: true).stdout(),
+    default_options: [
         'cpp_std=c++20',
         'b_lto=true',  # sets -flto
         'werror=true',  # sets -Werror
         'warning_level=3',  # level 3 sets -Wextra and -Wpedantic
     ]
 )
 
@@ -42,23 +42,23 @@
 
 libcommon = static_library(
     'common',
     [
         SRC_DIR / 'CostEvaluator.cpp',
         SRC_DIR / 'DynamicBitset.cpp',
         SRC_DIR / 'ProblemData.cpp',
-        SRC_DIR / 'XorShift128.cpp',
+        SRC_DIR / 'RandomNumberGenerator.cpp',
         SRC_DIR / 'Solution.cpp',
         SRC_DIR / 'SubPopulation.cpp',
+        SRC_DIR / 'TimeWindowSegment.cpp',
         SRC_DIR / 'crossover' / 'selective_route_exchange.cpp',
         SRC_DIR / 'crossover' / 'crossover.cpp',
         SRC_DIR / 'diversity' / 'broken_pairs_distance.cpp',
         SRC_DIR / 'search' / 'LocalSearch.cpp',
         SRC_DIR / 'search' / 'Route.cpp',
-        SRC_DIR / 'search' / 'Node.cpp',
         SRC_DIR / 'search' / 'MoveTwoClientsReversed.cpp',
         SRC_DIR / 'search' / 'TwoOpt.cpp',
         SRC_DIR / 'search' / 'RelocateStar.cpp',
         SRC_DIR / 'search' / 'SwapStar.cpp',
     ],
     include_directories: INCLUDES,
 )
@@ -67,28 +67,45 @@
 py = import('python').find_installation()
 dependencies = [py.dependency(), dependency('pybind11')]
 
 # Extension as [extension name, subdirectory]. The 'extension name' names the
 # eventual module name, and 'subdirectory' gives the source and installation 
 # directories (relative to SRC_DIR and INST_DIR).
 extensions = [
-    ['_pyvrp', ''],
-    ['_crossover', 'crossover'],
-    ['_diversity', 'diversity'],
-    ['_search', 'search'],
+    ['pyvrp', ''],
+    ['crossover', 'crossover'],
+    ['diversity', 'diversity'],
+    ['search', 'search'],
 ]
 
 foreach extension : extensions
-    name = extension[0]
+    rawname = extension[0]
+    name = '_' + rawname
     subdir = extension[1]
 
-    message('Going to build ' + subdir / name)
+    message('Going to build extension module ' + subdir / name + '.')
+
+    # Specify a custom target that generates the documentation header for this
+    # extension, of the form "<name>_docs.h". It is generated from headers in
+    # the relevant source directory - which the command below grabs for us.
+    doc_glob = f'import glob; print(*glob.glob("@SRC_DIR@/@subdir@/*.h"))'
+    doc_cmd = run_command('python', '-c', doc_glob, check: true)
+    doc_input_headers = doc_cmd.stdout().split()
+    doc_output_header = custom_target(
+        'docs for ' + name,
+        output: rawname + '_docs.h',
+        input: ['extract_docstrings.py'] + doc_input_headers,
+        command: ['python', '@INPUT@', '@OUTPUT@'],
+        depend_files: [SRC_DIR / subdir / 'bindings.cpp'],
+    )
+
+    # Register extension module to build.
     py.extension_module(
         name,
-        SRC_DIR / subdir / 'bindings.cpp',
+        [SRC_DIR / subdir / 'bindings.cpp', doc_output_header],
         dependencies: dependencies,
         link_with: libcommon,
         install: true,
         subdir: INST_DIR / subdir,
         include_directories: INCLUDES,
     )
 endforeach
```

### Comparing `pyvrp-0.4.4/pyproject.toml` & `pyvrp-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyvrp"
-version = "0.4.4"
+version = "0.5.0"
 description = "A state-of-the-art vehicle routing problem solver."
 authors = [
     "Niels Wouda <nielswouda@gmail.com>",
     "Leon Lan <leon.lanyidong@gmail.com>",
     "Wouter Kool <wouter.kool@ortec.com>",
 ]
 license = "MIT"
@@ -51,21 +51,18 @@
 
 
 [tool.poetry.group.docs]
 optional = true
 
 
 [tool.poetry.group.docs.dependencies]
-tomli = ">=2.0.1"
 nbsphinx = ">=0.8.9"
 ipython = ">=8.6.0"
 numpydoc = ">=1.5.0"
-sphinx_rtd_theme = ">=0.5.1"
-sphinx-autoapi = ">=2.0.1"
-docutils = "==0.16"
+sphinx-immaterial = ">=0.11.6"
 
 
 [tool.poetry.group.examples]
 optional = true
 
 
 [tool.poetry.group.examples.dependencies]
@@ -76,46 +73,58 @@
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 pytest = ">=6.0.0"
 pytest-cov = ">=2.6.1"
 codecov = "*"
 
 # These are used in the build script: for compiling the library (meson, ninja)
-# and for generating type stubs (mypy).
+# and for generating doc or type stubs (docblock, mypy).
 meson = "^1.0.0"
 ninja = "^1.11.1"
 mypy = "^0.991"
+docblock = "^0.0.5"
 
 
 [tool.poetry.scripts]
 pyvrp = "pyvrp.cli:main"
 
 
 [tool.black]
 line-length = 79
 
 
-[tool.isort]
-case_sensitive = true
-line_length = 79
-profile = "black"
+[tool.ruff]
+line-length = 79
+select = [
+    "E", "F", "I", "NPY", "PYI", "Q", "RET", "RSE", "RUF", "SLF", "SIM", "TCH"
+]
+
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]  # unused imports
+
+
+[tool.ruff.isort]
+case-sensitive = true
+known-first-party = ["pyvrp"]
 
 
 [tool.mypy]
 ignore_missing_imports = true
 
 
 [tool.pytest.ini_options]
 addopts = "--cov=. --cov-report=xml --cov-report=term"
 testpaths = "pyvrp"
 
 
 [tool.coverage.run]
 omit = [
     "build_extensions.py",  # build entrypoint
+    "extract_docstrings.py",  # build script
     "pyvrp/show_versions.py",  # only prints debug information
     "pyvrp/cli.py",  # tested in other ways than unit tests
     "*/tests/*",
     "venv/*",
     "docs/*",
 ]
 
@@ -138,10 +147,11 @@
 
 [tool.poetry.build]
 generate-setup-file = false
 script = "build_extensions.py"
 
 
 [build-system]
-# We need meson and ninja to build the C++ extensions.
-requires = ["poetry", "meson", "ninja"]
+# We need meson and ninja to build the C++ extensions, and docblock to extract
+# documentation for the extensions.
+requires = ["poetry", "meson", "ninja", "docblock"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyvrp-0.4.4/pyvrp/GeneticAlgorithm.py` & `pyvrp-0.5.0/pyvrp/GeneticAlgorithm.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,42 +4,68 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Callable, Collection, Tuple
 
 from .Result import Result
 from .Statistics import Statistics
 
 if TYPE_CHECKING:
-    from pyvrp.search.LocalSearch import LocalSearch
-    from pyvrp.stop import StoppingCriterion
+    from pyvrp.search.SearchMethod import SearchMethod
+    from pyvrp.stop.StoppingCriterion import StoppingCriterion
 
     from .PenaltyManager import PenaltyManager
     from .Population import Population
-    from ._pyvrp import CostEvaluator, ProblemData, Solution, XorShift128
+    from ._pyvrp import (
+        CostEvaluator,
+        ProblemData,
+        RandomNumberGenerator,
+        Solution,
+    )
 
     _Parents = Tuple[Solution, Solution]
     CrossoverOperator = Callable[
-        [_Parents, ProblemData, CostEvaluator, XorShift128], Solution
+        [_Parents, ProblemData, CostEvaluator, RandomNumberGenerator], Solution
     ]
 
 
 @dataclass
 class GeneticAlgorithmParams:
+    """
+    Parameters for the genetic algorithm.
+
+    Parameters
+    ----------
+    repair_probability
+        Probability (in :math:`[0, 1]`) of repairing an infeasible solution.
+        If the reparation makes the solution feasible, it is also added to
+        the population in the same iteration.
+    nb_iter_no_improvement
+        Number of iterations without any improvement needed before a restart
+        occurs.
+
+    Attributes
+    ----------
+    repair_probability
+        Probability of repairing an infeasible solution.
+    nb_iter_no_improvement
+        Number of iterations without improvement before a restart occurs.
+
+    Raises
+    ------
+    ValueError
+        When ``repair_probability`` is not in :math:`[0, 1]`, or
+        ``nb_iter_no_improvement`` is negative.
+    """
+
     repair_probability: float = 0.80
-    collect_statistics: bool = False
-    intensify_probability: float = 0.15
-    intensify_on_best: bool = True
     nb_iter_no_improvement: int = 20_000
 
     def __post_init__(self):
         if not 0 <= self.repair_probability <= 1:
             raise ValueError("repair_probability must be in [0, 1].")
 
-        if not 0 <= self.intensify_probability <= 1:
-            raise ValueError("intensify_probability must be in [0, 1].")
-
         if self.nb_iter_no_improvement < 0:
             raise ValueError("nb_iter_no_improvement < 0 not understood.")
 
 
 class GeneticAlgorithm:
     """
     Creates a GeneticAlgorithm instance.
@@ -50,16 +76,16 @@
         Data object describing the problem to be solved.
     penalty_manager
         Penalty manager to use.
     rng
         Random number generator.
     population
         Population to use.
-    local_search
-        Local search instance to use.
+    search_method
+        Search method to use.
     crossover_op
         Crossover operator to use for generating offspring.
     initial_solutions
         Initial solutions to use to initialise the population.
     params
         Genetic algorithm parameters. If not provided, a default will be used.
 
@@ -69,30 +95,30 @@
         When the population is empty.
     """
 
     def __init__(
         self,
         data: ProblemData,
         penalty_manager: PenaltyManager,
-        rng: XorShift128,
+        rng: RandomNumberGenerator,
         population: Population,
-        local_search: LocalSearch,
+        search_method: SearchMethod,
         crossover_op: CrossoverOperator,
         initial_solutions: Collection[Solution],
         params: GeneticAlgorithmParams = GeneticAlgorithmParams(),
     ):
         if len(initial_solutions) == 0:
             raise ValueError("Expected at least one initial solution.")
 
         self._data = data
         self._pm = penalty_manager
         self._rng = rng
         self._pop = population
-        self._ls = local_search
-        self._op = crossover_op
+        self._search = search_method
+        self._crossover = crossover_op
         self._initial_solutions = initial_solutions
         self._params = params
 
         # Find best feasible initial solution if any exist, else set a random
         # infeasible solution (with infinite cost) as the initial best.
         self._best = min(initial_solutions, key=self._cost_evaluator.cost)
 
@@ -132,82 +158,54 @@
 
                 for sol in self._initial_solutions:
                     self._pop.add(sol, self._cost_evaluator)
 
             curr_best = self._cost_evaluator.cost(self._best)
 
             parents = self._pop.select(self._rng, self._cost_evaluator)
-            offspring = self._op(
+            offspring = self._crossover(
                 parents, self._data, self._cost_evaluator, self._rng
             )
-            self._search(offspring)
+            self._improve_offspring(offspring)
 
             new_best = self._cost_evaluator.cost(self._best)
 
             if new_best < curr_best:
                 iters_no_improvement = 1
             else:
                 iters_no_improvement += 1
 
-            if self._params.collect_statistics:
-                stats.collect_from(self._pop, self._cost_evaluator)
+            stats.collect_from(self._pop, self._cost_evaluator)
 
         end = time.perf_counter() - start
         return Result(self._best, stats, iters, end)
 
-    def _search(self, sol: Solution):
+    def _improve_offspring(self, sol: Solution):
         def is_new_best(sol):
             cost = self._cost_evaluator.cost(sol)
             best_cost = self._cost_evaluator.cost(self._best)
             return cost < best_cost
 
         def add_and_register(sol):
             self._pop.add(sol, self._cost_evaluator)
             self._pm.register_load_feasible(not sol.has_excess_load())
             self._pm.register_time_feasible(not sol.has_time_warp())
 
-        intensify_prob = self._params.intensify_probability
-        should_intensify = self._rng.rand() < intensify_prob
-
-        sol = self._ls.run(sol, self._cost_evaluator, should_intensify)
+        sol = self._search(sol, self._cost_evaluator)
+        add_and_register(sol)
 
         if is_new_best(sol):
             self._best = sol
 
-            # Only intensify feasible, new best solutions. See also the repair
-            # step below. TODO Refactor to on_best callback (see issue #111)
-            if self._params.intensify_on_best:
-                sol = self._ls.intensify(
-                    sol, self._cost_evaluator, overlap_tolerance_degrees=360
-                )
-
-                if is_new_best(sol):
-                    self._best = sol
-
-        add_and_register(sol)
-
         # Possibly repair if current solution is infeasible. In that case, we
         # penalise infeasibility more using a penalty booster.
         if (
             not sol.is_feasible()
             and self._rng.rand() < self._params.repair_probability
         ):
-            should_intensify = self._rng.rand() < intensify_prob
-            sol = self._ls.run(
-                sol, self._pm.get_booster_cost_evaluator(), should_intensify
-            )
-
-            if is_new_best(sol):
-                self._best = sol
-
-                if self._params.intensify_on_best:
-                    sol = self._ls.intensify(
-                        sol,
-                        self._pm.get_booster_cost_evaluator(),
-                        overlap_tolerance_degrees=360,
-                    )
-
-                    if is_new_best(sol):
-                        self._best = sol
+            sol = self._search(sol, self._pm.get_booster_cost_evaluator())
 
             if sol.is_feasible():
                 add_and_register(sol)
+
+            if is_new_best(sol):
+                self._best = sol
```

### Comparing `pyvrp-0.4.4/pyvrp/Model.py` & `pyvrp-0.5.0/pyvrp/Model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from typing import List, Union
 from warnings import warn
 
 import numpy as np
 
-from pyvrp.GeneticAlgorithm import GeneticAlgorithm, GeneticAlgorithmParams
+from pyvrp.GeneticAlgorithm import GeneticAlgorithm
 from pyvrp.PenaltyManager import PenaltyManager
 from pyvrp.Population import Population, PopulationParams
 from pyvrp.Result import Result
 from pyvrp._pyvrp import (
     Client,
     ProblemData,
+    RandomNumberGenerator,
     Solution,
     VehicleType,
-    XorShift128,
 )
 from pyvrp.constants import MAX_USER_VALUE, MAX_VALUE
 from pyvrp.crossover import selective_route_exchange as srex
 from pyvrp.diversity import broken_pairs_distance as bpd
 from pyvrp.exceptions import ScalingWarning
 from pyvrp.stop import StoppingCriterion
 
 Depot = Client
 
 
 class Edge:
+    """
+    Stores an edge connecting two locations.
+    """
+
     __slots__ = ["frm", "to", "distance", "duration"]
 
     def __init__(self, frm: Client, to: Client, distance: int, duration: int):
         self.frm = frm
         self.to = to
         self.distance = distance
         self.duration = duration
@@ -208,21 +212,23 @@
         """
         Creates and returns a :class:`~pyvrp._pyvrp.ProblemData` instance
         from this model's attributes.
         """
         locs = self.locations
         loc2idx = {id(loc): idx for idx, loc in enumerate(locs)}
 
-        max_data_value = max(max(e.distance, e.duration) for e in self._edges)
-        if max_data_value > MAX_USER_VALUE:
-            msg = """
-            The maximum distance or duration value is very large. This might
-            impact numerical stability. Consider rescaling your input data.
-            """
-            warn(msg, ScalingWarning)
+        if self._edges:
+            max_value = max(max(e.distance, e.duration) for e in self._edges)
+
+            if max_value > MAX_USER_VALUE:
+                msg = """
+                The maximum distance or duration value is very large. This may
+                impact numerical stability. Consider rescaling your input data.
+                """
+                warn(msg, ScalingWarning)
 
         # Default value is a sufficiently large value to make sure any edges
         # not set below are never traversed.
         distances = np.full((len(locs), len(locs)), MAX_VALUE, dtype=int)
         durations = np.full((len(locs), len(locs)), MAX_VALUE, dtype=int)
 
         for edge in self._edges:
@@ -255,15 +261,15 @@
             NODE_OPERATORS,
             ROUTE_OPERATORS,
             LocalSearch,
             compute_neighbours,
         )
 
         data = self.data()
-        rng = XorShift128(seed=seed)
+        rng = RandomNumberGenerator(seed=seed)
         ls = LocalSearch(data, rng, compute_neighbours(data))
 
         for node_op in NODE_OPERATORS:
             ls.add_node_operator(node_op(data))
 
         for route_op in ROUTE_OPERATORS:
             ls.add_route_operator(route_op(data))
@@ -272,11 +278,10 @@
         pop_params = PopulationParams()
         pop = Population(bpd, pop_params)
         init = [
             Solution.make_random(data, rng)
             for _ in range(pop_params.min_pop_size)
         ]
 
-        gen_params = GeneticAlgorithmParams(collect_statistics=True)
-        gen_args = (data, pm, rng, pop, ls, srex, init, gen_params)
+        gen_args = (data, pm, rng, pop, ls, srex, init)
         algo = GeneticAlgorithm(*gen_args)  # type: ignore
         return algo.run(stop)
```

### Comparing `pyvrp-0.4.4/pyvrp/PenaltyManager.py` & `pyvrp-0.5.0/pyvrp/PenaltyManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,26 +29,25 @@
         Number of feasibility registrations between penalty value updates. The
         penalty manager updates the penalty terms every once in a while based
         on recent feasibility registrations. This parameter controls how often
         such updating occurs.
     penalty_increase
         Amount :math:`p_i \\ge 1` by which the current penalties are
         increased when insufficient feasible solutions (see
-        :py:attr:`~target_feasible`) have been found amongst the most recent
+        ``target_feasible``) have been found amongst the most recent
         registrations. The penalty values :math:`v` are updated as
         :math:`v \\gets p_i v`.
     penalty_decrease
         Amount :math:`p_d \\in [0, 1]` by which the current penalties are
-        decreased when sufficient feasible solutions (see
-        :py:attr:`~target_feasible`) have been found amongst the most recent
-        registrations. The penalty values :math:`v` are updated as
-        :math:`v \\gets p_d v`.
+        decreased when sufficient feasible solutions (see ``target_feasible``)
+        have been found amongst the most recent registrations. The penalty
+        values :math:`v` are updated as :math:`v \\gets p_d v`.
     target_feasible
         Target percentage :math:`p_f \\in [0, 1]` of feasible registrations
-        in the last :py:attr:`~num_registrations_between_penalty_updates`
+        in the last ``num_registrations_between_penalty_updates``
         registrations. This percentage is used to update the penalty terms:
         when insufficient feasible solutions have been registered, the
         penalties are increased; similarly, when too many feasible solutions
         have been registered, the penalty terms are decreased. This ensures a
         balanced population, with a fraction :math:`p_f` feasible and a
         fraction :math:`1 - p_f` infeasible solutions.
 
@@ -61,24 +60,23 @@
     repair_booster
         A repair booster value.
     num_registrations_between_penalty_updates
         Number of feasibility registrations between penalty value updates.
     penalty_increase
         Amount :math:`p_i \\ge 1` by which the current penalties are
         increased when insufficient feasible solutions (see
-        :py:attr:`~target_feasible`) have been found amongst the most recent
+        ``target_feasible``) have been found amongst the most recent
         registrations.
     penalty_decrease
         Amount :math:`p_d \\in [0, 1]` by which the current penalties are
-        decreased when sufficient feasible solutions (see
-        :py:attr:`~target_feasible`) have been found amongst the most recent
-        registrations.
+        decreased when sufficient feasible solutions (see ``target_feasible``)
+        have been found amongst the most recent registrations.
     target_feasible
         Target percentage :math:`p_f \\in [0, 1]` of feasible registrations
-        in the last :py:attr:`~num_registrations_between_penalty_updates`
+        in the last ``num_registrations_between_penalty_updates``
         registrations.
     """
 
     init_capacity_penalty: int = 20
     init_time_warp_penalty: int = 6
     repair_booster: int = 12
     num_registrations_between_penalty_updates: int = 50
@@ -152,16 +150,16 @@
 
         # +- 1 to ensure we do not get stuck at the same integer values,
         # bounded to [1, 1000] to avoid overflow in cost computations.
         if diff > 0:
             return int(
                 min(self._params.penalty_increase * penalty + 1, 1000.0)
             )
-        else:
-            return int(max(self._params.penalty_decrease * penalty - 1, 1.0))
+
+        return int(max(self._params.penalty_decrease * penalty - 1, 1.0))
 
     def register_load_feasible(self, is_load_feasible: bool):
         """
         Registers another capacity feasibility result. The current load penalty
         is updated once sufficiently many results have been gathered.
 
         Parameters
```

### Comparing `pyvrp-0.4.4/pyvrp/Population.py` & `pyvrp-0.5.0/pyvrp/Population.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from __future__ import annotations
 
-from typing import Callable, Generator, Tuple
+from typing import TYPE_CHECKING, Callable, Generator, Tuple
 from warnings import warn
 
-from ._pyvrp import (
-    CostEvaluator,
-    PopulationParams,
-    Solution,
-    SubPopulation,
-    XorShift128,
-)
+from ._pyvrp import PopulationParams, SubPopulation
 from .exceptions import EmptySolutionWarning
 
+if TYPE_CHECKING:
+    from ._pyvrp import CostEvaluator, RandomNumberGenerator, Solution
+
 
 class Population:
     """
     Creates a Population instance.
 
     Parameters
     ----------
@@ -119,15 +116,15 @@
             """
             warn(msg, EmptySolutionWarning)
 
         # Note: the CostEvaluator is required here since adding a solution
         # may trigger a purge which needs to compute the biased fitness which
         # requires computing the cost.
         if solution.is_feasible():
-            # Note: the feasible subpopulation actually doet not depend
+            # Note: the feasible subpopulation actually does not depend
             # on the penalty values but we use the same implementation.
             self._feas.add(solution, cost_evaluator)
         else:
             self._infeas.add(solution, cost_evaluator)
 
     def clear(self):
         """
@@ -135,15 +132,15 @@
         population.
         """
         self._feas = SubPopulation(self._op, self._params)
         self._infeas = SubPopulation(self._op, self._params)
 
     def select(
         self,
-        rng: XorShift128,
+        rng: RandomNumberGenerator,
         cost_evaluator: CostEvaluator,
         k: int = 2,
     ) -> Tuple[Solution, Solution]:
         """
         Selects two (if possible non-identical) parents by tournament, subject
         to a diversity restriction.
 
@@ -176,15 +173,18 @@
             tries += 1
             second = self._get_tournament(rng, k)
             diversity = self._op(first, second)
 
         return first, second
 
     def get_tournament(
-        self, rng: XorShift128, cost_evaluator: CostEvaluator, k: int = 2
+        self,
+        rng: RandomNumberGenerator,
+        cost_evaluator: CostEvaluator,
+        k: int = 2,
     ) -> Solution:
         """
         Selects a solution from this population by k-ary tournament, based
         on the (internal) fitness values of the selected solutions.
 
         Parameters
         ----------
@@ -200,15 +200,15 @@
         -------
         Solution
             The selected solution.
         """
         self._update_fitness(cost_evaluator)
         return self._get_tournament(rng, k)
 
-    def _get_tournament(self, rng: XorShift128, k: int) -> Solution:
+    def _get_tournament(self, rng: RandomNumberGenerator, k: int) -> Solution:
         if k <= 0:
             raise ValueError(f"Expected k > 0; got k = {k}.")
 
         def select():
             num_feas = len(self._feas)
             idx = rng.randint(len(self))
```

### Comparing `pyvrp-0.4.4/pyvrp/Statistics.py` & `pyvrp-0.5.0/pyvrp/Statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,19 @@
 
         self.runtimes.append(self._clock - start)
         self.num_iterations += 1
 
         # The following lines access private members of the population, but in
         # this case that is mostly OK: we really want to have that access to
         # enable detailed statistics logging.
-        feas_subpop = population._feas  # noqa
+        feas_subpop = population._feas  # noqa: SLF001
         feas_datum = self._collect_from_subpop(feas_subpop, cost_evaluator)
         self.feas_stats.append(feas_datum)
 
-        infeas_subpop = population._infeas  # noqa
+        infeas_subpop = population._infeas  # noqa: SLF001
         infeas_datum = self._collect_from_subpop(infeas_subpop, cost_evaluator)
         self.infeas_stats.append(infeas_datum)
 
     def _collect_from_subpop(
         self, subpop: SubPopulation, cost_evaluator: CostEvaluator
     ) -> _Datum:
         if not subpop:  # empty, so many statistics cannot be collected
@@ -180,15 +180,15 @@
 
         infeas_data = [
             {f: v for f, v in zip(infeas_fields, vars(datum).values())}
             for datum in self.infeas_stats
         ]
 
         with open(where, "w") as fh:
-            header = ["runtime"] + feas_fields + infeas_fields
+            header = ["runtime", *feas_fields, *infeas_fields]
             writer = csv.DictWriter(
                 fh, header, delimiter=delimiter, quoting=quoting, **kwargs
             )
 
             writer.writeheader()
 
             for idx in range(self.num_iterations):
```

### Comparing `pyvrp-0.4.4/pyvrp/cli.py` & `pyvrp-0.5.0/pyvrp/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 import numpy as np
 
 try:
     import tomli
     from tqdm import tqdm
     from tqdm.contrib.concurrent import process_map
-except ModuleNotFoundError:
+except ModuleNotFoundError as exc:
     msg = "Install 'tqdm' and 'tomli' to use the command line program."
-    raise ModuleNotFoundError(msg)
+    raise ModuleNotFoundError(msg) from exc
 
 import pyvrp.search
 from pyvrp import (
     GeneticAlgorithm,
     GeneticAlgorithmParams,
     PenaltyManager,
     PenaltyParams,
     Population,
     PopulationParams,
+    RandomNumberGenerator,
     Result,
     Solution,
-    XorShift128,
 )
 from pyvrp.crossover import selective_route_exchange as srex
 from pyvrp.diversity import broken_pairs_distance as bpd
 from pyvrp.read import INSTANCE_FORMATS, ROUND_FUNCS, read
 from pyvrp.search import (
     NODE_OPERATORS,
     ROUTE_OPERATORS,
@@ -51,24 +51,24 @@
 
     header = [
         "  ".join(f"{hdr:<{ln}s}" for ln, hdr in zip(lens, headers)),
         "  ".join("-" * ln for ln in lens),
     ]
 
     content = [
-        "  ".join(f"{str(c):>{ln}s}" for ln, c in zip(lens, r)) for r in rows
+        "  ".join(f"{c!s:>{ln}s}" for ln, c in zip(lens, r)) for r in rows
     ]
 
     return "\n".join(header + content)
 
 
 def maybe_mkdir(where: str):
     if where:
-        stats_dir = Path(where)
-        stats_dir.mkdir(parents=True, exist_ok=True)
+        path = Path(where)
+        path.mkdir(parents=True, exist_ok=True)
 
 
 def solve(
     data_loc: str,
     instance_format: str,
     round_func: str,
     seed: int,
@@ -96,16 +96,15 @@
     max_runtime
         Maximum runtime (in seconds) for solving. Either ``max_runtime`` or
         ``max_iterations`` must be specified.
     max_iterations
         Maximum number of iterations for solving. Either ``max_runtime`` or
         ``max_iterations`` must be specified.
     stats_dir
-        The directory to write runtime statistics to. Enables statistics
-        collection when passed.
+        The directory to write runtime statistics to.
     sol_dir
         The directory to write the best found solutions to.
 
     Returns
     -------
     Result
         Object storing the solver outcome.
@@ -113,26 +112,20 @@
     if kwargs.get("config_loc"):
         with open(kwargs["config_loc"], "rb") as fh:
             config = tomli.load(fh)
     else:
         config = {}
 
     gen_params = GeneticAlgorithmParams(**config.get("genetic", {}))
-
-    if stats_dir:
-        # The statistics directory argument trumps whatever we got earlier
-        # from the configuration file.
-        gen_params.collect_statistics = True
-
     pen_params = PenaltyParams(**config.get("penalty", {}))
     pop_params = PopulationParams(**config.get("population", {}))
     nb_params = NeighbourhoodParams(**config.get("neighbourhood", {}))
 
     data = read(data_loc, instance_format, round_func)
-    rng = XorShift128(seed=seed)
+    rng = RandomNumberGenerator(seed=seed)
     pen_manager = PenaltyManager(pen_params)
     pop = Population(bpd, params=pop_params)
 
     neighbours = compute_neighbours(data, nb_params)
     ls = LocalSearch(data, rng, neighbours)
 
     node_ops = NODE_OPERATORS
@@ -250,16 +243,14 @@
     """
     parser = argparse.ArgumentParser(prog="pyvrp", description=description)
 
     parser.add_argument("instances", nargs="+", help="Instance paths.")
 
     msg = """
     Directory to store runtime statistics in, as CSV files (one per instance).
-    If passed, this enables collecting runtime statistics (default False), at
-    a slight performance hit.
     """
     parser.add_argument("--stats_dir", help=msg)
 
     msg = """
     Directory to store best observed solutions in, in VRPLIB format (one file
     per instance).
     """
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/DynamicBitset.cpp` & `pyvrp-0.5.0/pyvrp/cpp/DynamicBitset.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/cpp/DynamicBitset.h` & `pyvrp-0.5.0/pyvrp/cpp/DynamicBitset.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/cpp/Matrix.h` & `pyvrp-0.5.0/pyvrp/cpp/Matrix.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/cpp/Measure.h` & `pyvrp-0.5.0/pyvrp/cpp/Measure.h`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         return std::hash<pyvrp::Value>()(measure.get());
 #endif
     }
 };
 
 template <pyvrp::MeasureType Type> class numeric_limits<pyvrp::Measure<Type>>
 {
-public:  // TODO should return type be Measure<Type>?
+public:
     static pyvrp::Value max()
     {
         return std::numeric_limits<pyvrp::Value>::max();
     }
 
     static pyvrp::Value min()
     {
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/README.md` & `pyvrp-0.5.0/pyvrp/cpp/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,7 +12,12 @@
 
 ## Bindings
 
 We use `pybind11` to generate Python bindings for the C++ codebase. These
 bindings are generated from the `bindings.cpp` source files of each folder. 
 Each `bindings.cpp` file is compiled into a single extension module named after
 the installation folder, prefixed with an underscore.
+
+The bindings depend on header files ending in `_docs.h`. Those header files
+contain docstrings that are automatically extracted from the other header files
+present in this directory. The documentation headers are generated automatically
+by Meson during compilation.
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/Solution.cpp` & `pyvrp-0.5.0/pyvrp/cpp/Solution.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #include "Solution.h"
 #include "ProblemData.h"
+#include "TimeWindowSegment.h"
 
 #include <fstream>
 #include <numeric>
 #include <unordered_map>
 
 using pyvrp::Cost;
 using pyvrp::Distance;
@@ -41,15 +42,20 @@
 Routes const &Solution::getRoutes() const { return routes_; }
 
 std::vector<std::pair<Client, Client>> const &Solution::getNeighbours() const
 {
     return neighbours;
 }
 
-bool Solution::isFeasible() const { return !hasExcessLoad() && !hasTimeWarp(); }
+bool Solution::isFeasible() const
+{
+    return !hasExcessLoad() && !hasTimeWarp() && isComplete();
+}
+
+bool Solution::isComplete() const { return numMissingClients_ == 0; }
 
 bool Solution::hasExcessLoad() const { return excessLoad_ > 0; }
 
 bool Solution::hasTimeWarp() const { return timeWarp_ > 0; }
 
 Distance Solution::distance() const { return distance_; }
 
@@ -97,15 +103,15 @@
     for (auto const &route : other.routes_)
         if (client2vehType[route.visits()[0]] != route.vehicleType())
             return false;
 
     return true;
 }
 
-Solution::Solution(ProblemData const &data, XorShift128 &rng)
+Solution::Solution(ProblemData const &data, RandomNumberGenerator &rng)
     : neighbours(data.numClients() + 1, {0, 0})
 {
     // Shuffle clients (to create random routes)
     auto clients = std::vector<int>(data.numClients());
     std::iota(clients.begin(), clients.end(), 1);
     std::shuffle(clients.begin(), clients.end(), rng);
 
@@ -156,109 +162,96 @@
     }
 
     std::vector<size_t> visits(data.numClients() + 1, 0);
     std::vector<size_t> usedVehicles(data.numVehicleTypes(), 0);
     for (auto const &route : routes)
     {
         if (route.empty())
-        {
-            auto const msg = "Solution should not contain empty routes.";
-            throw std::runtime_error(msg);
-        }
+            throw std::runtime_error("Solution should not have empty routes.");
 
         usedVehicles[route.vehicleType()]++;
         for (auto const client : route)
             visits[client]++;
     }
 
-    for (size_t vehType = 0; vehType != data.numVehicleTypes(); vehType++)
-        if (usedVehicles[vehType] > data.vehicleType(vehType).numAvailable)
-        {
-            std::ostringstream msg;
-            auto const numAvailable = data.vehicleType(vehType).numAvailable;
-            msg << "Used more than " << numAvailable << " vehicles of type "
-                << vehType << '.';
-            throw std::runtime_error(msg.str());
-        }
-
     for (size_t client = 1; client <= data.numClients(); ++client)
     {
         if (data.client(client).required && visits[client] == 0)
+            numMissingClients_ += 1;
+
+        if (visits[client] > 1)
         {
             std::ostringstream msg;
-            msg << "Client " << client << " is required but not present.";
+            msg << "Client " << client << " is visited more than once.";
             throw std::runtime_error(msg.str());
         }
+    }
 
-        if (visits[client] > 1)
+    for (size_t vehType = 0; vehType != data.numVehicleTypes(); vehType++)
+        if (usedVehicles[vehType] > data.vehicleType(vehType).numAvailable)
         {
             std::ostringstream msg;
-            msg << "Client " << client << " is visited more than once.";
+            auto const numAvailable = data.vehicleType(vehType).numAvailable;
+            msg << "Used more than " << numAvailable << " vehicles of type "
+                << vehType << '.';
             throw std::runtime_error(msg.str());
         }
-    }
 
     makeNeighbours();
     evaluate(data);
 }
 
 Solution::Route::Route(ProblemData const &data,
-                       Visits const visits,
+                       Visits visits,
                        size_t const vehicleType)
     : visits_(std::move(visits)), centroid_({0, 0}), vehicleType_(vehicleType)
 {
     if (visits_.empty())
         return;
 
-    for (size_t idx = 0; idx != size(); ++idx)
-        release_ = std::max(release_, data.client(visits_[idx]).releaseTime);
-
-    Duration time = std::max(release_, data.depot().twEarly);
-    int prevClient = 0;
+    auto const &vehType = data.vehicleType(vehicleType);
+    auto const &depot = data.client(vehType.depot);
+    auto const &durMat = data.durationMatrix();
+
+    TimeWindowSegment depotTws(vehType.depot, depot);
+    auto tws = depotTws;
+    size_t prevClient = vehType.depot;
 
     for (size_t idx = 0; idx != size(); ++idx)
     {
-        auto const &clientData = data.client(visits_[idx]);
+        auto const client = visits_[idx];
+        auto const &clientData = data.client(client);
 
-        distance_ += data.dist(prevClient, visits_[idx]);
-        duration_ += data.duration(prevClient, visits_[idx]);
+        distance_ += data.dist(prevClient, client);
+        travel_ += data.duration(prevClient, client);
         demand_ += clientData.demand;
         service_ += clientData.serviceDuration;
         prizes_ += clientData.prize;
 
         centroid_.first += static_cast<double>(clientData.x) / size();
         centroid_.second += static_cast<double>(clientData.y) / size();
 
-        time += data.client(prevClient).serviceDuration
-                + data.duration(prevClient, visits_[idx]);
-
-        if (time < clientData.twEarly)  // add wait duration
-        {
-            wait_ += clientData.twEarly - time;
-            time = clientData.twEarly;
-        }
-
-        if (time > clientData.twLate)  // add time warp
-        {
-            timeWarp_ += time - clientData.twLate;
-            time = clientData.twLate;
-        }
+        auto const clientTws = TimeWindowSegment(client, clientData);
+        tws = TimeWindowSegment::merge(durMat, tws, clientTws);
 
-        prevClient = visits_[idx];
+        prevClient = client;
     }
 
     Client const last = visits_.back();  // last client has depot as successor
-    distance_ += data.dist(last, 0);
-    duration_ += data.duration(last, 0);
+    distance_ += data.dist(last, vehType.depot);
+    travel_ += data.duration(last, vehType.depot);
 
-    time += data.client(last).serviceDuration + data.duration(last, 0);
-    timeWarp_ += std::max<Duration>(time - data.depot().twLate, 0);
+    excessLoad_ = std::max<Load>(demand_ - vehType.capacity, 0);
 
-    auto const capacity = data.vehicleType(vehicleType).capacity;
-    excessLoad_ = capacity < demand_ ? demand_ - capacity : 0;
+    tws = TimeWindowSegment::merge(durMat, tws, depotTws);
+    duration_ = tws.duration();
+    startTime_ = tws.twEarly();
+    slack_ = tws.twLate() - tws.twEarly();
+    timeWarp_ = tws.totalTimeWarp();
+    release_ = tws.releaseTime();
 }
 
 bool Solution::Route::empty() const { return visits_.empty(); }
 
 size_t Solution::Route::size() const { return visits_.size(); }
 
 Client Solution::Route::operator[](size_t idx) const { return visits_[idx]; }
@@ -266,36 +259,43 @@
 Visits::const_iterator Solution::Route::begin() const
 {
     return visits_.cbegin();
 }
 
 Visits::const_iterator Solution::Route::end() const { return visits_.cend(); }
 
-Visits::const_iterator Solution::Route::cbegin() const
-{
-    return visits_.cbegin();
-}
-
-Visits::const_iterator Solution::Route::cend() const { return visits_.cend(); }
-
 Visits const &Solution::Route::visits() const { return visits_; }
 
 Distance Solution::Route::distance() const { return distance_; }
 
 Load Solution::Route::demand() const { return demand_; }
 
 Load Solution::Route::excessLoad() const { return excessLoad_; }
 
 Duration Solution::Route::duration() const { return duration_; }
 
 Duration Solution::Route::serviceDuration() const { return service_; }
 
 Duration Solution::Route::timeWarp() const { return timeWarp_; }
 
-Duration Solution::Route::waitDuration() const { return wait_; }
+Duration Solution::Route::waitDuration() const
+{
+    return duration_ - travel_ - service_;
+}
+
+Duration Solution::Route::travelDuration() const { return travel_; }
+
+Duration Solution::Route::startTime() const { return startTime_; }
+
+Duration Solution::Route::endTime() const
+{
+    return startTime_ + duration_ - timeWarp_;
+}
+
+Duration Solution::Route::slack() const { return slack_; }
 
 Duration Solution::Route::releaseTime() const { return release_; }
 
 Cost Solution::Route::prizes() const { return prizes_; }
 
 std::pair<double, double> const &Solution::Route::centroid() const
 {
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/SubPopulation.cpp` & `pyvrp-0.5.0/pyvrp/cpp/SubPopulation.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/cpp/crossover/crossover.cpp` & `pyvrp-0.5.0/pyvrp/cpp/crossover/crossover.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,17 @@
     auto const &clientData = data.client(client);
     auto const &prevData = data.client(prev);
 
     auto const clientService = clientData.serviceDuration;
     auto const clientLate = clientData.twLate;
     auto const nextLate = data.client(next).twLate;
 
-    // Determine the earliest time we can depart from prev.
-    auto const prevStart = std::max(data.duration(0, prev), prevData.twEarly);
-    auto const prevFinish = prevStart + prevData.serviceDuration;
-
-    // Time warp when we go directly from prev to next (current situation).
+    // Determine the earliest time we can depart from prev, and compute the
+    // time warp when we go directly from prev to next (current situation).
+    auto const prevFinish = prevData.twEarly + prevData.serviceDuration;
     auto const prevNextArrive = prevFinish + data.duration(prev, next);
     auto const currTimeWarp = std::max<Duration>(prevNextArrive - nextLate, 0);
 
     // Determine arrival at client. This incurs some timewarp if the arrival is
     // after client.twLate. We finish at start time + service. We subtract any
     // time warp from the departure time at client.
     auto const clientArrive = prevFinish + data.duration(prev, client);
@@ -113,21 +111,21 @@
         auto offset = 0;
         for (size_t idx = 0; idx <= route.size() && !route.empty(); ++idx)
         {
             Client prev, next;
 
             if (idx == 0)  // try after depot
             {
-                prev = 0;
+                prev = 0;  // TODO hardcoded depot
                 next = route[0];
             }
             else if (idx == route.size())  // try before depot
             {
                 prev = route.back();
-                next = 0;
+                next = 0;  // TODO hardcoded depot
             }
             else  // try between [idx - 1] and [idx]
             {
                 prev = route[idx - 1];
                 next = route[idx];
             }
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/crossover/crossover.h` & `pyvrp-0.5.0/pyvrp/cpp/crossover/crossover.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #ifndef PYVRP_CROSSOVER_H
 #define PYVRP_CROSSOVER_H
 
 #include "CostEvaluator.h"
 #include "DynamicBitset.h"
 #include "ProblemData.h"
 #include "Solution.h"
-#include "XorShift128.h"
 
 #include <functional>
 #include <vector>
 
 namespace pyvrp::crossover
 {
 /**
@@ -34,19 +33,16 @@
  * @param parents          The parent solutions.
  * @param data             The problem data.
  * @param costEvaluator    The cost evaluator.
  * @param startIndices     Start indices of routes in parent solutions.
  * @param numMovedRoutes   Number of routes to move.
  * @return A new offspring.
  *
- * <br />
- * Yuichi Nagata and Shigenobu Kobayashi. "A memetic algorithm for
- * the pickup and delivery problem with time windows using selective route
- * exchange crossover". In: International Conference on Parallel Problem Solving
- * from Nature. Springer. 2010, pp. 536–545.
+ * Note that this is an internal docstring: the SREX operator is wrapped on
+ * the Python side.
  */
 Solution selectiveRouteExchange(
     std::pair<Solution const *, Solution const *> const &parents,
     ProblemData const &data,
     CostEvaluator const &costEvaluator,
     std::pair<size_t, size_t> const startIndices,
     size_t const numMovedRoutes);
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/crossover/selective_route_exchange.cpp` & `pyvrp-0.5.0/pyvrp/cpp/crossover/selective_route_exchange.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,17 @@
 using Routes = std::vector<Route>;
 
 namespace
 {
 // Angle of the given route w.r.t. the centroid of all client locations.
 double routeAngle(pyvrp::ProblemData const &data, Route const &route)
 {
-    // This computes a pseudo-angle that sorts roughly equivalently to the atan2
-    // angle, but is much faster to compute. See the following post for details:
-    // https://stackoverflow.com/a/16561333/4316405.
     auto const [dataX, dataY] = data.centroid();
     auto const [routeX, routeY] = route.centroid();
-    auto const dx = routeX - dataX;
-    auto const dy = routeY - dataY;
-    return std::copysign(1. - dx / (std::fabs(dx) + std::fabs(dy)), dy);
+    return std::atan2(routeY - dataY, routeX - dataX);
 }
 
 Routes sortByAscAngle(pyvrp::ProblemData const &data, Routes routes)
 {
     auto cmp = [&data](Route a, Route b) {
         return routeAngle(data, a) < routeAngle(data, b);
     };
@@ -227,14 +222,15 @@
     std::vector<Solution::Route> routes2;
     routes2.reserve(nRoutesA);
 
     for (size_t r = 0; r < nRoutesA; r++)
     {
         if (!visits1[r].empty())
             routes1.emplace_back(data, visits1[r], routesA[r].vehicleType());
+
         if (!visits2[r].empty())
             routes2.emplace_back(data, visits2[r], routesA[r].vehicleType());
     }
 
     Solution sol1{data, routes1};
     Solution sol2{data, routes2};
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/diversity/broken_pairs_distance.cpp` & `pyvrp-0.5.0/pyvrp/cpp/diversity/broken_pairs_distance.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/Exchange.h` & `pyvrp-0.5.0/pyvrp/cpp/search/Exchange.h`

 * *Files 10% similar despite different names*

```diff
@@ -4,86 +4,93 @@
 #include "LocalSearchOperator.h"
 #include "TimeWindowSegment.h"
 
 #include <cassert>
 
 namespace pyvrp::search
 {
-using TWS = TimeWindowSegment;
-
 /**
- * Template class that exchanges N consecutive nodes from U's route (starting at
- * U) with M consecutive nodes from V's route (starting at V). As special cases,
- * (1, 0) is pure relocate, and (1, 1) pure swap.
+ * Exchange()
+ *
+ * The :math:`(N, M)`-exchange operators exhange :math:`N` consecutive clients
+ * from :math:`U`'s route (starting at :math:`U`) with :math:`M` consecutive
+ * clients from :math:`V`'s route (starting at :math:`V`). This includes
+ * the RELOCATE and SWAP operators as special cases.
+ *
+ * The :math:`(N, M)`-exchange class uses C++ templates for different :math:`N`
+ * and :math:`M` to efficiently evaluate these moves.
  */
-template <size_t N, size_t M> class Exchange : public LocalSearchOperator<Node>
+template <size_t N, size_t M>
+class Exchange : public LocalSearchOperator<Route::Node>
 {
     using LocalSearchOperator::LocalSearchOperator;
 
     static_assert(N >= M && N > 0, "N < M or N == 0 does not make sense");
 
     // Tests if the segment starting at node of given length contains the depot
-    inline bool containsDepot(Node *node, size_t segLength) const;
+    inline bool containsDepot(Route::Node *node, size_t segLength) const;
 
     // Tests if the segments of U and V overlap in the same route
-    inline bool overlap(Node *U, Node *V) const;
+    inline bool overlap(Route::Node *U, Route::Node *V) const;
 
     // Tests if the segments of U and V are adjacent in the same route
-    inline bool adjacent(Node *U, Node *V) const;
+    inline bool adjacent(Route::Node *U, Route::Node *V) const;
 
     // Special case that's applied when M == 0
-    Cost evalRelocateMove(Node *U,
-                          Node *V,
+    Cost evalRelocateMove(Route::Node *U,
+                          Route::Node *V,
                           CostEvaluator const &costEvaluator) const;
 
     // Applied when M != 0
-    Cost
-    evalSwapMove(Node *U, Node *V, CostEvaluator const &costEvaluator) const;
+    Cost evalSwapMove(Route::Node *U,
+                      Route::Node *V,
+                      CostEvaluator const &costEvaluator) const;
 
 public:
-    Cost
-    evaluate(Node *U, Node *V, CostEvaluator const &costEvaluator) override;
+    Cost evaluate(Route::Node *U,
+                  Route::Node *V,
+                  CostEvaluator const &costEvaluator) override;
 
-    void apply(Node *U, Node *V) const override;
+    void apply(Route::Node *U, Route::Node *V) const override;
 };
 
 template <size_t N, size_t M>
-bool Exchange<N, M>::containsDepot(Node *node, size_t segLength) const
+bool Exchange<N, M>::containsDepot(Route::Node *node, size_t segLength) const
 {
     if (node->isDepot())
         return true;
 
     // size() is the position of the last node in the route. So the segment
     // must include the depot if position + move length - 1 (-1 since we're
     // also moving the node *at* position) is larger than size().
     return node->position + segLength - 1 > node->route->size();
 }
 
 template <size_t N, size_t M>
-bool Exchange<N, M>::overlap(Node *U, Node *V) const
+bool Exchange<N, M>::overlap(Route::Node *U, Route::Node *V) const
 {
     return U->route == V->route
            // We need max(M, 1) here because when V is the depot and M == 0,
            // this would turn negative and wrap around to a large number.
            && U->position <= V->position + std::max<size_t>(M, 1) - 1
            && V->position <= U->position + N - 1;
 }
 
 template <size_t N, size_t M>
-bool Exchange<N, M>::adjacent(Node *U, Node *V) const
+bool Exchange<N, M>::adjacent(Route::Node *U, Route::Node *V) const
 {
     if (U->route != V->route)
         return false;
 
     return U->position + N == V->position || V->position + M == U->position;
 }
 
 template <size_t N, size_t M>
-Cost Exchange<N, M>::evalRelocateMove(Node *U,
-                                      Node *V,
+Cost Exchange<N, M>::evalRelocateMove(Route::Node *U,
+                                      Route::Node *V,
                                       CostEvaluator const &costEvaluator) const
 {
     auto const posU = U->position;
     auto const posV = V->position;
 
     assert(posU > 0);
     auto *endU = N == 1 ? U : (*U->route)[posU + N - 1];
@@ -99,15 +106,15 @@
     Cost deltaCost = static_cast<Cost>(proposed - current);
 
     if (U->route != V->route)
     {
         if (U->route->isFeasible() && deltaCost >= 0)
             return deltaCost;
 
-        auto uTWS = TWS::merge(
+        auto uTWS = TimeWindowSegment::merge(
             data.durationMatrix(), p(U)->twBefore, n(endU)->twAfter);
 
         deltaCost += costEvaluator.twPenalty(uTWS.totalTimeWarp());
         deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
 
         auto const loadDiff = U->route->loadBetween(posU, posU + N - 1);
 
@@ -120,59 +127,62 @@
             return deltaCost;  // even without V, the move will never be good.
 
         deltaCost += costEvaluator.loadPenalty(V->route->load() + loadDiff,
                                                V->route->capacity());
         deltaCost -= costEvaluator.loadPenalty(V->route->load(),
                                                V->route->capacity());
 
-        auto vTWS = TWS::merge(data.durationMatrix(),
-                               V->twBefore,
-                               U->route->twBetween(posU, posU + N - 1),
-                               n(V)->twAfter);
+        auto vTWS
+            = TimeWindowSegment::merge(data.durationMatrix(),
+                                       V->twBefore,
+                                       U->route->twBetween(posU, posU + N - 1),
+                                       n(V)->twAfter);
 
         deltaCost += costEvaluator.twPenalty(vTWS.totalTimeWarp());
         deltaCost -= costEvaluator.twPenalty(V->route->timeWarp());
     }
     else  // within same route
     {
         auto const *route = U->route;
 
         if (!route->hasTimeWarp() && deltaCost >= 0)
             return deltaCost;
 
         if (posU < posV)
         {
-            auto const tws = TWS::merge(data.durationMatrix(),
-                                        p(U)->twBefore,
-                                        route->twBetween(posU + N, posV),
-                                        route->twBetween(posU, posU + N - 1),
-                                        n(V)->twAfter);
+            auto const tws
+                = TimeWindowSegment::merge(data.durationMatrix(),
+                                           p(U)->twBefore,
+                                           route->twBetween(posU + N, posV),
+                                           route->twBetween(posU, posU + N - 1),
+                                           n(V)->twAfter);
 
             deltaCost += costEvaluator.twPenalty(tws.totalTimeWarp());
         }
         else
         {
-            auto const tws = TWS::merge(data.durationMatrix(),
-                                        V->twBefore,
-                                        route->twBetween(posU, posU + N - 1),
-                                        route->twBetween(posV + 1, posU - 1),
-                                        n(endU)->twAfter);
+            auto const tws
+                = TimeWindowSegment::merge(data.durationMatrix(),
+                                           V->twBefore,
+                                           route->twBetween(posU, posU + N - 1),
+                                           route->twBetween(posV + 1, posU - 1),
+                                           n(endU)->twAfter);
 
             deltaCost += costEvaluator.twPenalty(tws.totalTimeWarp());
         }
 
         deltaCost -= costEvaluator.twPenalty(route->timeWarp());
     }
 
     return deltaCost;
 }
 
 template <size_t N, size_t M>
-Cost Exchange<N, M>::evalSwapMove(Node *U,
-                                  Node *V,
+Cost Exchange<N, M>::evalSwapMove(Route::Node *U,
+                                  Route::Node *V,
                                   CostEvaluator const &costEvaluator) const
 {
     auto const posU = U->position;
     auto const posV = V->position;
 
     assert(posU > 0 && posV > 0);
     auto *endU = N == 1 ? U : (*U->route)[posU + N - 1];
@@ -196,35 +206,37 @@
     Cost deltaCost = static_cast<Cost>(proposed - current);
 
     if (U->route != V->route)
     {
         if (U->route->isFeasible() && V->route->isFeasible() && deltaCost >= 0)
             return deltaCost;
 
-        auto uTWS = TWS::merge(data.durationMatrix(),
-                               p(U)->twBefore,
-                               V->route->twBetween(posV, posV + M - 1),
-                               n(endU)->twAfter);
+        auto uTWS
+            = TimeWindowSegment::merge(data.durationMatrix(),
+                                       p(U)->twBefore,
+                                       V->route->twBetween(posV, posV + M - 1),
+                                       n(endU)->twAfter);
 
         deltaCost += costEvaluator.twPenalty(uTWS.totalTimeWarp());
         deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
 
         auto const loadU = U->route->loadBetween(posU, posU + N - 1);
         auto const loadV = V->route->loadBetween(posV, posV + M - 1);
         auto const loadDiff = loadU - loadV;
 
         deltaCost += costEvaluator.loadPenalty(U->route->load() - loadDiff,
                                                U->route->capacity());
         deltaCost -= costEvaluator.loadPenalty(U->route->load(),
                                                U->route->capacity());
 
-        auto vTWS = TWS::merge(data.durationMatrix(),
-                               p(V)->twBefore,
-                               U->route->twBetween(posU, posU + N - 1),
-                               n(endV)->twAfter);
+        auto vTWS
+            = TimeWindowSegment::merge(data.durationMatrix(),
+                                       p(V)->twBefore,
+                                       U->route->twBetween(posU, posU + N - 1),
+                                       n(endV)->twAfter);
 
         deltaCost += costEvaluator.twPenalty(vTWS.totalTimeWarp());
         deltaCost -= costEvaluator.twPenalty(V->route->timeWarp());
 
         deltaCost += costEvaluator.loadPenalty(V->route->load() + loadDiff,
                                                V->route->capacity());
         deltaCost -= costEvaluator.loadPenalty(V->route->load(),
@@ -235,44 +247,46 @@
         auto const *route = U->route;
 
         if (!route->hasTimeWarp() && deltaCost >= 0)
             return deltaCost;
 
         if (posU < posV)
         {
-            auto const tws = TWS::merge(data.durationMatrix(),
-                                        p(U)->twBefore,
-                                        route->twBetween(posV, posV + M - 1),
-                                        route->twBetween(posU + N, posV - 1),
-                                        route->twBetween(posU, posU + N - 1),
-                                        n(endV)->twAfter);
+            auto const tws
+                = TimeWindowSegment::merge(data.durationMatrix(),
+                                           p(U)->twBefore,
+                                           route->twBetween(posV, posV + M - 1),
+                                           route->twBetween(posU + N, posV - 1),
+                                           route->twBetween(posU, posU + N - 1),
+                                           n(endV)->twAfter);
 
             deltaCost += costEvaluator.twPenalty(tws.totalTimeWarp());
         }
         else
         {
-            auto const tws = TWS::merge(data.durationMatrix(),
-                                        p(V)->twBefore,
-                                        route->twBetween(posU, posU + N - 1),
-                                        route->twBetween(posV + M, posU - 1),
-                                        route->twBetween(posV, posV + M - 1),
-                                        n(endU)->twAfter);
+            auto const tws
+                = TimeWindowSegment::merge(data.durationMatrix(),
+                                           p(V)->twBefore,
+                                           route->twBetween(posU, posU + N - 1),
+                                           route->twBetween(posV + M, posU - 1),
+                                           route->twBetween(posV, posV + M - 1),
+                                           n(endU)->twAfter);
 
             deltaCost += costEvaluator.twPenalty(tws.totalTimeWarp());
         }
 
         deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
     }
 
     return deltaCost;
 }
 
 template <size_t N, size_t M>
-Cost Exchange<N, M>::evaluate(Node *U,
-                              Node *V,
+Cost Exchange<N, M>::evaluate(Route::Node *U,
+                              Route::Node *V,
                               CostEvaluator const &costEvaluator)
 {
     if (containsDepot(U, N) || overlap(U, V))
         return 0;
 
     if constexpr (M > 0)
         if (containsDepot(V, M))
@@ -294,15 +308,16 @@
         if (adjacent(U, V))
             return 0;
 
         return evalSwapMove(U, V, costEvaluator);
     }
 }
 
-template <size_t N, size_t M> void Exchange<N, M>::apply(Node *U, Node *V) const
+template <size_t N, size_t M>
+void Exchange<N, M>::apply(Route::Node *U, Route::Node *V) const
 {
     auto *uToInsert = N == 1 ? U : (*U->route)[U->position + N - 1];
     auto *insertUAfter = M == 0 ? V : (*V->route)[V->position + M - 1];
 
     // Insert these 'extra' nodes of U after the end of V...
     for (size_t count = 0; count != N - M; ++count)
     {
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/LocalSearch.cpp` & `pyvrp-0.5.0/pyvrp/cpp/search/LocalSearch.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,70 @@
 #include "LocalSearch.h"
 #include "Measure.h"
 #include "TimeWindowSegment.h"
 
 #include <algorithm>
 #include <cassert>
 #include <numeric>
-#include <set>
 #include <stdexcept>
 #include <vector>
 
 using pyvrp::Solution;
 using pyvrp::search::LocalSearch;
 using TWS = pyvrp::TimeWindowSegment;
 
-Solution LocalSearch::search(Solution &solution,
+Solution LocalSearch::operator()(Solution const &solution,
+                                 CostEvaluator const &costEvaluator)
+{
+    loadSolution(solution);
+
+    while (true)
+    {
+        search(costEvaluator);
+
+        // When numMoves != 0, search() modified the currently loaded solution.
+        // In that case we need to reload the solution because intensify()'s
+        // route operators need to update their caches.
+        // TODO remove this.
+        if (numMoves != 0)
+        {
+            Solution const newSol = exportSolution();
+            loadSolution(newSol);
+        }
+
+        intensify(costEvaluator);
+
+        if (numMoves == 0)  // then the current solution is locally optimal.
+            break;
+    }
+
+    return exportSolution();
+}
+
+Solution LocalSearch::search(Solution const &solution,
                              CostEvaluator const &costEvaluator)
 {
     loadSolution(solution);
+    search(costEvaluator);
+    return exportSolution();
+}
 
+Solution LocalSearch::intensify(Solution const &solution,
+                                CostEvaluator const &costEvaluator,
+                                double overlapTolerance)
+{
+    loadSolution(solution);
+    intensify(costEvaluator, overlapTolerance);
+    return exportSolution();
+}
+
+void LocalSearch::search(CostEvaluator const &costEvaluator)
+{
     if (nodeOps.empty())
-        throw std::runtime_error("No known node operators.");
+        return;
 
     // Caches the last time nodes were tested for modification (uses numMoves to
     // track this). The lastModified field, in contrast, track when a route was
     // last *actually* modified.
     std::vector<int> lastTestedNodes(data.numClients() + 1, -1);
     lastModified = std::vector<int>(data.numVehicles(), 0);
 
@@ -41,16 +82,14 @@
 
             auto const lastTestedNode = lastTestedNodes[uClient];
             lastTestedNodes[uClient] = numMoves;
 
             if (U->route && !data.client(uClient).required)  // test removing U
                 maybeRemove(U, costEvaluator);
 
-            // Shuffling the neighbours in this loop should not matter much as
-            // we are already randomizing the nodes U.
             for (auto const vClient : neighbours[uClient])
             {
                 auto *V = &clients[vClient];
 
                 if (!U->route && V->route)             // U might be inserted
                     maybeInsert(U, V, costEvaluator);  // into V's route
 
@@ -80,35 +119,31 @@
                     auto empty = std::find_if(begin, end, pred);
                     begin = end;
 
                     if (empty == end)
                         continue;
 
                     if (U->route)  // try inserting U into the empty route.
-                        applyNodeOps(U, empty->depot, costEvaluator);
+                        applyNodeOps(U, &empty->startDepot, costEvaluator);
                     else  // U is not in the solution, so again try inserting.
-                        maybeInsert(U, empty->depot, costEvaluator);
+                        maybeInsert(U, &empty->startDepot, costEvaluator);
                 }
             }
         }
     }
-
-    return exportSolution();
 }
 
-Solution LocalSearch::intensify(Solution &solution,
-                                CostEvaluator const &costEvaluator,
-                                int overlapToleranceDegrees)
+void LocalSearch::intensify(CostEvaluator const &costEvaluator,
+                            double overlapTolerance)
 {
-    loadSolution(solution);
-
-    auto const overlapTolerance = overlapToleranceDegrees * 65536;
+    if (overlapTolerance < 0 || overlapTolerance > 1)
+        throw std::runtime_error("overlapTolerance must be in [0, 1].");
 
     if (routeOps.empty())
-        throw std::runtime_error("No known route operators.");
+        return;
 
     std::vector<int> lastTestedRoutes(data.numVehicles(), -1);
     lastModified = std::vector<int>(data.numVehicles(), 0);
 
     searchCompleted = false;
     numMoves = 0;
 
@@ -122,16 +157,14 @@
 
             if (U.empty())
                 continue;
 
             auto const lastTested = lastTestedRoutes[U.idx];
             lastTestedRoutes[U.idx] = numMoves;
 
-            // Shuffling in this loop should not matter much as we are
-            // already randomizing the routes U.
             for (size_t rV = 0; rV != U.idx; ++rV)
             {
                 auto &V = routes[rV];
 
                 if (V.empty() || !U.overlapsWith(V, overlapTolerance))
                     continue;
 
@@ -140,29 +173,27 @@
 
                 if (lastModifiedRoute > lastTested
                     && applyRouteOps(&U, &V, costEvaluator))
                     continue;
             }
         }
     }
-
-    return exportSolution();
 }
 
-void LocalSearch::shuffle(XorShift128 &rng)
+void LocalSearch::shuffle(RandomNumberGenerator &rng)
 {
     std::shuffle(orderNodes.begin(), orderNodes.end(), rng);
     std::shuffle(nodeOps.begin(), nodeOps.end(), rng);
 
     std::shuffle(orderRoutes.begin(), orderRoutes.end(), rng);
     std::shuffle(routeOps.begin(), routeOps.end(), rng);
 }
 
-bool LocalSearch::applyNodeOps(Node *U,
-                               Node *V,
+bool LocalSearch::applyNodeOps(Route::Node *U,
+                               Route::Node *V,
                                CostEvaluator const &costEvaluator)
 {
     for (auto *nodeOp : nodeOps)
         if (nodeOp->evaluate(U, V, costEvaluator) < 0)
         {
             auto *routeU = U->route;  // copy pointers because the operator can
             auto *routeV = V->route;  // modify the node's route membership
@@ -194,16 +225,16 @@
 
             return true;
         }
 
     return false;
 }
 
-void LocalSearch::maybeInsert(Node *U,
-                              Node *V,
+void LocalSearch::maybeInsert(Route::Node *U,
+                              Route::Node *V,
                               CostEvaluator const &costEvaluator)
 {
     assert(!U->route && V->route);
 
     Distance const deltaDist = data.dist(V->client, U->client)
                                + data.dist(U->client, n(V)->client)
                                - data.dist(V->client, n(V)->client);
@@ -230,15 +261,16 @@
     if (deltaCost < 0)
     {
         U->insertAfter(V);           // U has no route, so there's nothing to
         update(V->route, V->route);  // update there.
     }
 }
 
-void LocalSearch::maybeRemove(Node *U, CostEvaluator const &costEvaluator)
+void LocalSearch::maybeRemove(Route::Node *U,
+                              CostEvaluator const &costEvaluator)
 {
     assert(U->route);
 
     Distance const deltaDist = data.dist(p(U)->client, n(U)->client)
                                - data.dist(p(U)->client, U->client)
                                - data.dist(U->client, n(U)->client);
 
@@ -277,113 +309,106 @@
         V->update();
         lastModified[V->idx] = numMoves;
     }
 }
 
 void LocalSearch::loadSolution(Solution const &solution)
 {
+    if (!solution.isComplete())  // TODO allow incomplete at some point
+        throw std::runtime_error("LocalSearch requires complete solutions.");
+
     for (size_t client = 0; client <= data.numClients(); client++)
     {
-        clients[client].tw = {static_cast<int>(client),  // TODO cast
-                              static_cast<int>(client),  // TODO cast
-                              data.client(client).serviceDuration,
-                              0,
-                              data.client(client).twEarly,
-                              data.client(client).twLate,
-                              data.client(client).releaseTime};
-
+        clients[client].tw = {client, data.client(client)};
         clients[client].route = nullptr;  // nullptr implies "not in solution"
     }
 
     // First empty all routes
-    for (size_t r = 0; r != data.numVehicles(); r++)
+    for (auto &route : routes)
     {
-        Node *startDepot = &startDepots[r];
-        Node *endDepot = &endDepots[r];
+        auto const &vehicleType = data.vehicleType(route.vehicleType());
+
+        auto *startDepot = &route.startDepot;
+        auto *endDepot = &route.endDepot;
 
         startDepot->prev = endDepot;
         startDepot->next = endDepot;
 
         endDepot->prev = startDepot;
         endDepot->next = startDepot;
 
-        startDepot->tw = clients[0].tw;
-        startDepot->twBefore = clients[0].tw;
+        startDepot->tw = clients[vehicleType.depot].tw;
+        startDepot->twBefore = clients[vehicleType.depot].tw;
 
-        endDepot->tw = clients[0].tw;
-        endDepot->twAfter = clients[0].tw;
+        endDepot->tw = clients[vehicleType.depot].tw;
+        endDepot->twAfter = clients[vehicleType.depot].tw;
     }
 
     // Determine offsets for vehicle types.
     std::vector<size_t> vehicleOffset(data.numVehicleTypes(), 0);
     for (size_t vehType = 1; vehType < data.numVehicleTypes(); vehType++)
     {
-        auto const available = data.vehicleType(vehType).numAvailable;
-        vehicleOffset[vehType] = vehicleOffset[vehType - 1] + available;
+        auto const prevAvail = data.vehicleType(vehType - 1).numAvailable;
+        vehicleOffset[vehType] = vehicleOffset[vehType - 1] + prevAvail;
     }
 
     // Load routes from solution.
     for (auto const &solRoute : solution.getRoutes())
     {
         // Determine index of next route of this type to load, where we rely
         // on solution to be valid to not exceed the number of vehicles per
         // vehicle type.
         auto const r = vehicleOffset[solRoute.vehicleType()]++;
         Route *route = &routes[r];
-        Node *startDepot = &startDepots[r];
-        Node *endDepot = &endDepots[r];
 
-        Node *client = &clients[solRoute[0]];
+        auto *client = &clients[solRoute[0]];
         client->route = route;
 
-        client->prev = startDepot;
-        startDepot->next = client;
+        client->prev = &route->startDepot;
+        route->startDepot.next = client;
 
         for (size_t idx = 1; idx < solRoute.size(); idx++)
         {
-            Node *prev = client;
+            auto *prev = client;
 
             client = &clients[solRoute[idx]];
             client->route = route;
 
             client->prev = prev;
             prev->next = client;
         }
 
-        client->next = endDepot;
-        endDepot->prev = client;
+        client->next = &route->endDepot;
+        route->endDepot.prev = client;
     }
 
     for (auto &route : routes)
         route.update();
 
     for (auto *routeOp : routeOps)
         routeOp->init(solution);
 }
 
 Solution LocalSearch::exportSolution() const
 {
     std::vector<Solution::Route> solRoutes;
     solRoutes.reserve(data.numVehicles());
 
-    for (size_t r = 0; r < data.numVehicles(); r++)
+    for (auto const &route : routes)
     {
-        if (routes[r].empty())
+        if (route.empty())
             continue;
 
         std::vector<int> visits;
-        Node *node = startDepots[r].next;
+        visits.reserve(route.size());
 
-        while (!node->isDepot())
-        {
+        for (auto *node : route)
             visits.push_back(node->client);
-            node = node->next;
-        }
 
-        solRoutes.emplace_back(data, visits, routes[r].vehicleType());
+        solRoutes.emplace_back(data, visits, route.vehicleType());
     }
 
     return {data, solRoutes};
 }
 
 void LocalSearch::addNodeOperator(NodeOp &op) { nodeOps.emplace_back(&op); }
 
@@ -406,57 +431,46 @@
         {
             throw std::runtime_error("Neighbourhood of client "
                                      + std::to_string(client)
                                      + " contains itself or the depot.");
         }
     }
 
-    auto isEmpty = [](auto const &neighbours) { return neighbours.empty(); };
-    if (std::all_of(neighbours.begin(), neighbours.end(), isEmpty))
-        throw std::runtime_error("Neighbourhood is empty.");
-
     this->neighbours = neighbours;
 }
 
 LocalSearch::Neighbours const &LocalSearch::getNeighbours() const
 {
     return neighbours;
 }
 
 LocalSearch::LocalSearch(ProblemData const &data, Neighbours neighbours)
     : data(data),
       neighbours(data.numClients() + 1),
       orderNodes(data.numClients()),
       orderRoutes(data.numVehicles()),
-      lastModified(data.numVehicles(), -1),
-      clients(data.numClients() + 1),
-      startDepots(data.numVehicles()),
-      endDepots(data.numVehicles())
+      lastModified(data.numVehicles(), -1)
 {
     setNeighbours(neighbours);
 
     std::iota(orderNodes.begin(), orderNodes.end(), 1);
     std::iota(orderRoutes.begin(), orderRoutes.end(), 0);
 
-    for (size_t i = 0; i <= data.numClients(); i++)
-        clients[i].client = i;
+    clients.reserve(data.numClients() + 1);
+    for (size_t client = 0; client <= data.numClients(); ++client)
+        clients.emplace_back(client);
 
     routes.reserve(data.numVehicles());
     size_t rIdx = 0;
-    for (size_t vehType = 0; vehType != data.numVehicleTypes(); ++vehType)
+    for (size_t vehTypeIdx = 0; vehTypeIdx != data.numVehicleTypes();
+         ++vehTypeIdx)
     {
-        auto const numAvailable = data.vehicleType(vehType).numAvailable;
+        auto const &vehType = data.vehicleType(vehTypeIdx);
+        auto const numAvailable = vehType.numAvailable;
+
         for (size_t i = 0; i != numAvailable; ++i)
         {
-            routes.emplace_back(data, rIdx, vehType);
-            routes[rIdx].depot = &startDepots[rIdx];
-
-            startDepots[rIdx].client = 0;
-            startDepots[rIdx].route = &routes[rIdx];
-
-            endDepots[rIdx].client = 0;
-            endDepots[rIdx].route = &routes[rIdx];
-
+            routes.emplace_back(data, rIdx, vehTypeIdx);
             rIdx++;
         }
     }
 }
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/LocalSearch.h` & `pyvrp-0.5.0/pyvrp/cpp/search/LocalSearch.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,80 @@
 #ifndef PYVRP_LOCALSEARCH_H
 #define PYVRP_LOCALSEARCH_H
 
 #include "CostEvaluator.h"
 #include "LocalSearchOperator.h"
-#include "Node.h"
 #include "ProblemData.h"
+#include "RandomNumberGenerator.h"
 #include "Route.h"
 #include "Solution.h"
-#include "XorShift128.h"
 
 #include <functional>
 #include <stdexcept>
 #include <vector>
 
 namespace pyvrp::search
 {
 class LocalSearch
 {
-    using NodeOp = LocalSearchOperator<Node>;
+    using NodeOp = LocalSearchOperator<Route::Node>;
     using RouteOp = LocalSearchOperator<Route>;
     using Neighbours = std::vector<std::vector<int>>;
 
     ProblemData const &data;
 
     // Neighborhood restrictions: list of nearby clients for each client (size
     // numClients + 1, but nothing stored for the depot!)
     Neighbours neighbours;
 
     std::vector<int> orderNodes;   // node order used by LocalSearch::search
     std::vector<int> orderRoutes;  // route order used by LocalSearch::intensify
 
     std::vector<int> lastModified;  // tracks when routes were last modified
 
-    std::vector<Node> clients;  // Note that clients[0] is a sentinel value
+    std::vector<Route::Node> clients;
     std::vector<Route> routes;
 
-    std::vector<Node> startDepots;  // These mark the start of routes
-    std::vector<Node> endDepots;    // These mark the end of routes
-
     std::vector<NodeOp *> nodeOps;
     std::vector<RouteOp *> routeOps;
 
     int numMoves = 0;              // Operator counter
     bool searchCompleted = false;  // No further improving move found?
 
     // Load an initial solution that we will attempt to improve.
     void loadSolution(Solution const &solution);
 
     // Export the LS solution back into a solution.
     Solution exportSolution() const;
 
     // Tests the node pair (U, V).
-    bool applyNodeOps(Node *U, Node *V, CostEvaluator const &costEvaluator);
+    bool applyNodeOps(Route::Node *U,
+                      Route::Node *V,
+                      CostEvaluator const &costEvaluator);
 
     // Tests the route pair (U, V).
     bool applyRouteOps(Route *U, Route *V, CostEvaluator const &costEvaluator);
 
     // Updates solution state after an improving local search move.
     void update(Route *U, Route *V);
 
     // Test inserting U after V. Called if U is not currently in the solution.
-    void maybeInsert(Node *U, Node *V, CostEvaluator const &costEvaluator);
+    void maybeInsert(Route::Node *U,
+                     Route::Node *V,
+                     CostEvaluator const &costEvaluator);
 
     // Test removing U from the solution. Called when U can be removed.
-    void maybeRemove(Node *U, CostEvaluator const &costEvaluator);
+    void maybeRemove(Route::Node *U, CostEvaluator const &costEvaluator);
+
+    // Performs search on the currently loaded solution.
+    void search(CostEvaluator const &costEvaluator);
+
+    // Performs intensify on the currently loaded solution.
+    void intensify(CostEvaluator const &costEvaluator,
+                   double overlapTolerance = 0.05);
 
 public:
     /**
      * Adds a local search operator that works on node/client pairs U and V.
      */
     void addNodeOperator(NodeOp &op);
 
@@ -86,31 +93,39 @@
 
     /**
      * @return The neighbourhood structure currently in use.
      */
     Neighbours const &getNeighbours() const;
 
     /**
+     * Iteratively calls ``search()`` and ``intensify()`` until no further
+     * improvements are made.
+     */
+    Solution operator()(Solution const &solution,
+                        CostEvaluator const &costEvaluator);
+
+    /**
      * Performs regular (node-based) local search around the given solution,
      * and returns a new, hopefully improved solution.
      */
-    Solution search(Solution &solution, CostEvaluator const &costEvaluator);
+    Solution search(Solution const &solution,
+                    CostEvaluator const &costEvaluator);
 
     /**
      * Performs a more intensive route-based local search around the given
      * solution, and returns a new, hopefully improved solution.
      */
-    Solution intensify(Solution &solution,
+    Solution intensify(Solution const &solution,
                        CostEvaluator const &costEvaluator,
-                       int overlapToleranceDegrees = 0);
+                       double overlapTolerance = 0.05);
 
     /**
      * Shuffles the order in which the node and route pairs are evaluated, and
      * the order in which node and route operators are applied.
      */
-    void shuffle(XorShift128 &rng);
+    void shuffle(RandomNumberGenerator &rng);
 
     LocalSearch(ProblemData const &data, Neighbours neighbours);
 };
 }  // namespace pyvrp::search
 
 #endif  // PYVRP_LOCALSEARCH_H
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/LocalSearchOperator.h` & `pyvrp-0.5.0/pyvrp/cpp/search/LocalSearchOperator.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #ifndef PYVRP_LOCALSEARCHOPERATOR_H
 #define PYVRP_LOCALSEARCHOPERATOR_H
 
 #include "CostEvaluator.h"
 #include "Measure.h"
-#include "Node.h"
 #include "ProblemData.h"
 #include "Route.h"
 #include "Solution.h"
 
 namespace pyvrp::search
 {
 template <typename Arg> class LocalSearchOperatorBase
 {
     // Can only be specialised into either a Node or Route operator; there
     // are no other types that are expected to work.
-    static_assert(std::is_same<Arg, Node>::value
+    static_assert(std::is_same<Arg, Route::Node>::value
                   || std::is_same<Arg, Route>::value);
 
 protected:
     ProblemData const &data;
 
 public:
     /**
@@ -48,15 +47,16 @@
 
 template <typename Arg>
 class LocalSearchOperator : public LocalSearchOperatorBase<Arg>
 {
 };
 
 template <>  // specialisation for node operators
-class LocalSearchOperator<Node> : public LocalSearchOperatorBase<Node>
+class LocalSearchOperator<Route::Node>
+    : public LocalSearchOperatorBase<Route::Node>
 {
     using LocalSearchOperatorBase::LocalSearchOperatorBase;
 };
 
 template <>  // specialisation for route operators
 class LocalSearchOperator<Route> : public LocalSearchOperatorBase<Route>
 {
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/MoveTwoClientsReversed.cpp` & `pyvrp-0.5.0/pyvrp/cpp/search/MoveTwoClientsReversed.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #include <cassert>
 
 using pyvrp::search::MoveTwoClientsReversed;
 using TWS = pyvrp::TimeWindowSegment;
 
 pyvrp::Cost MoveTwoClientsReversed::evaluate(
-    Node *U, Node *V, pyvrp::CostEvaluator const &costEvaluator)
+    Route::Node *U, Route::Node *V, pyvrp::CostEvaluator const &costEvaluator)
 {
     if (U == n(V) || n(U) == V || n(U)->isDepot())
         return 0;
 
     auto const posU = U->position;
     auto const posV = V->position;
 
@@ -91,14 +91,14 @@
 
         deltaCost -= costEvaluator.twPenalty(route->timeWarp());
     }
 
     return deltaCost;
 }
 
-void MoveTwoClientsReversed::apply(Node *U, Node *V) const
+void MoveTwoClientsReversed::apply(Route::Node *U, Route::Node *V) const
 {
     auto *X = n(U);  // copy since the insert below changes n(U)
 
     U->insertAfter(V);
     X->insertAfter(V);
 }
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/MoveTwoClientsReversed.h` & `pyvrp-0.5.0/pyvrp/cpp/search/MoveTwoClientsReversed.h`

 * *Files 27% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 #include "LocalSearchOperator.h"
 
 namespace pyvrp::search
 {
 /**
  * Inserts U -> X after V (as V -> X -> U), if that is an improving move.
  */
-class MoveTwoClientsReversed : public LocalSearchOperator<Node>
+class MoveTwoClientsReversed : public LocalSearchOperator<Route::Node>
 {
     using LocalSearchOperator::LocalSearchOperator;
 
 public:
-    Cost
-    evaluate(Node *U, Node *V, CostEvaluator const &costEvaluator) override;
+    Cost evaluate(Route::Node *U,
+                  Route::Node *V,
+                  CostEvaluator const &costEvaluator) override;
 
-    void apply(Node *U, Node *V) const override;
+    void apply(Route::Node *U, Route::Node *V) const override;
 };
 }  // namespace pyvrp::search
 
 #endif  // PYVRP_MOVETWOCLIENTSREVERSED_H
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/RelocateStar.cpp` & `pyvrp-0.5.0/pyvrp/cpp/search/RelocateStar.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 pyvrp::Cost RelocateStar::evaluate(Route *U,
                                    Route *V,
                                    pyvrp::CostEvaluator const &costEvaluator)
 {
     move = {};
 
-    for (auto *nodeU = n(U->depot); !nodeU->isDepot(); nodeU = n(nodeU))
+    for (auto *nodeU : *U)
     {
-        // Test inserting U after V's depot
-        Cost deltaCost = relocate.evaluate(nodeU, V->depot, costEvaluator);
+        // Test inserting U after V's start depot
+        Cost deltaCost
+            = relocate.evaluate(nodeU, &V->startDepot, costEvaluator);
 
         if (deltaCost < move.deltaCost)
-            move = {deltaCost, nodeU, V->depot};
+            move = {deltaCost, nodeU, &V->startDepot};
 
-        for (auto *nodeV = n(V->depot); !nodeV->isDepot(); nodeV = n(nodeV))
+        for (auto *nodeV : *V)
         {
             // Test inserting U after V
             deltaCost = relocate.evaluate(nodeU, nodeV, costEvaluator);
 
             if (deltaCost < move.deltaCost)
                 move = {deltaCost, nodeU, nodeV};
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/RelocateStar.h` & `pyvrp-0.5.0/pyvrp/cpp/search/RelocateStar.h`

 * *Files 19% similar despite different names*

```diff
@@ -11,16 +11,16 @@
  * ways: from U to V, and from V to U.
  */
 class RelocateStar : public LocalSearchOperator<Route>
 {
     struct Move
     {
         Cost deltaCost = 0;
-        Node *from = nullptr;
-        Node *to = nullptr;
+        Route::Node *from = nullptr;
+        Route::Node *to = nullptr;
     };
 
     Exchange<1, 0> relocate;
     Move move;
 
 public:
     Cost
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/Route.h` & `pyvrp-0.5.0/pyvrp/cpp/search/Route.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,84 @@
 #ifndef PYVRP_ROUTE_H
 #define PYVRP_ROUTE_H
 
-#include "CircleSector.h"
-#include "Node.h"
 #include "ProblemData.h"
 #include "TimeWindowSegment.h"
 
-#include <array>
-#include <bit>
 #include <cassert>
 #include <iosfwd>
 
 namespace pyvrp::search
 {
 class Route
 {
+public:
+    struct Node
+    {
+        // TODO rename client to location/loc
+        size_t client;           // Location represented by this node
+        size_t position = 0;     // Position in the route
+        Route *route = nullptr;  // Indicates membership of a route, if any.
+        Node *prev = nullptr;    // Predecessor in route
+        Node *next = nullptr;    // Successor in route
+
+        // TODO can these data fields be moved to Route?
+        Load cumulatedLoad = 0;          // Load depot -> client (incl)
+        Distance cumulatedDistance = 0;  // Dist depot - client (incl)
+
+        TimeWindowSegment tw;        // TWS for individual node (client)
+        TimeWindowSegment twBefore;  // TWS for (0...client) including self
+        TimeWindowSegment twAfter;   // TWS for (client...0) including self
+
+        Node(size_t client);
+
+        [[nodiscard]] inline bool isDepot() const;
+
+        /**
+         * Inserts this node after the other and updates the relevant links.
+         */
+        void insertAfter(Node *other);
+
+        /**
+         * Swaps this node with the other and updates the relevant links.
+         */
+        void swapWith(Node *other);
+
+        /**
+         * Removes this node and updates the relevant links.
+         */
+        void remove();
+    };
+
+private:
     ProblemData const &data;
     size_t const vehicleType_;
 
-    std::vector<Node *> nodes;  // List of nodes (in order) in this solution.
-    CircleSector sector;        // Circle sector of the route's clients
-
-    Load load_;            // Current route load.
-    bool isLoadFeasible_;  // Whether current load is feasible.
-
-    Duration timeWarp_;        // Current route time warp.
-    bool isTimeWarpFeasible_;  // Whether current time warp is feasible.
-
-    // Populates the nodes vector.
-    void setupNodes();
+    std::vector<Node *> nodes;  // List of nodes in this route, excl. depot
+    std::pair<double, double> centroid;  // Center point of route's clients.
 
-    // Sets the sector data.
-    void setupSector();
-
-    // Sets forward node time windows.
-    void setupRouteTimeWindows();
+    Load load_;          // Current route load.
+    Duration timeWarp_;  // Current route time warp.
 
 public:                // TODO make fields private
     size_t const idx;  // Route index
-    Node *depot;       // Pointer to the associated depot
+    Node startDepot;   // Departure depot for this route
+    Node endDepot;     // Return depot for this route
 
     /**
      * @return The client or depot node at the given position.
      */
     [[nodiscard]] inline Node *operator[](size_t position) const;
 
+    [[nodiscard]] inline std::vector<Node *>::const_iterator begin() const;
+    [[nodiscard]] inline std::vector<Node *>::const_iterator end() const;
+
+    [[nodiscard]] inline std::vector<Node *>::iterator begin();
+    [[nodiscard]] inline std::vector<Node *>::iterator end();
+
     /**
      * Tests if this route is feasible.
      *
      * @return true if the route is feasible, false otherwise.
      */
     [[nodiscard]] inline bool isFeasible() const;
 
@@ -73,22 +103,22 @@
 
     /**
      * @return Total time warp on this route.
      */
     [[nodiscard]] inline Duration timeWarp() const;
 
     /**
-     * @return true if this route is empty, false otherwise.
+     * @return The load capacity of this route.
      */
-    [[nodiscard]] inline bool empty() const;
+    [[nodiscard]] inline Load capacity() const;
 
     /**
-     * @return The load capacity of this route.
+     * @return true if this route is empty, false otherwise.
      */
-    [[nodiscard]] inline Load capacity() const;
+    [[nodiscard]] inline bool empty() const;
 
     /**
      * @return Number of clients in this route.
      */
     [[nodiscard]] inline size_t size() const;
 
     /**
@@ -109,94 +139,126 @@
 
     /**
      * @return This route's vehicle type.
      */
     [[nodiscard]] size_t vehicleType() const;
 
     /**
-     * Tests if this route overlaps with the other route, that is, whether
-     * their circle sectors overlap with a given tolerance.
+     * Tests if this route potentially overlaps with the other route, subject
+     * to a tolerance in [0, 1].
      */
-    [[nodiscard]] bool overlapsWith(Route const &other,
-                                    int const tolerance) const;
+    [[nodiscard]] bool overlapsWith(Route const &other, double tolerance) const;
 
     /**
      * Updates this route. To be called after swapping nodes/changing the
      * solution.
      */
     void update();
 
     Route(ProblemData const &data, size_t const idx, size_t const vehType);
 };
 
+/**
+ * Convenience method accessing the node directly before the argument.
+ */
+inline Route::Node *p(Route::Node *node) { return node->prev; }
+
+/**
+ * Convenience method accessing the node directly after the argument.
+ */
+inline Route::Node *n(Route::Node *node) { return node->next; }
+
+bool Route::Node::isDepot() const
+{
+    // We need to be in a route to be the depot. If we are, then we need to
+    // be either the route's start or end depot.
+    return route && (this == &route->startDepot || this == &route->endDepot);
+}
+
 bool Route::isFeasible() const { return !hasExcessLoad() && !hasTimeWarp(); }
 
-bool Route::hasExcessLoad() const { return !isLoadFeasible_; }
+bool Route::hasExcessLoad() const { return load_ > capacity(); }
 
 bool Route::hasTimeWarp() const
 {
 #ifdef PYVRP_NO_TIME_WINDOWS
     return false;
 #else
-    return !isTimeWarpFeasible_;
+    return timeWarp_ > 0;
 #endif
 }
 
-Node *Route::operator[](size_t position) const
+Route::Node *Route::operator[](size_t position) const
 {
     assert(position > 0);
     return nodes[position - 1];
 }
 
+std::vector<Route::Node *>::const_iterator Route::begin() const
+{
+    return nodes.begin();
+}
+std::vector<Route::Node *>::const_iterator Route::end() const
+{
+    return nodes.end();
+}
+
+std::vector<Route::Node *>::iterator Route::begin() { return nodes.begin(); }
+std::vector<Route::Node *>::iterator Route::end() { return nodes.end(); }
+
 Load Route::load() const { return load_; }
 
 Duration Route::timeWarp() const { return timeWarp_; }
 
-bool Route::empty() const { return size() == 0; }
-
 Load Route::capacity() const { return data.vehicleType(vehicleType_).capacity; }
 
-size_t Route::size() const
-{
-    return nodes.size() - 1;  // exclude end depot
-}
+bool Route::empty() const { return size() == 0; }
+
+size_t Route::size() const { return nodes.size(); }
 
 TimeWindowSegment Route::twBetween(size_t start, size_t end) const
 {
-    assert(0 < start && start <= end && end <= nodes.size());
+    assert(0 < start && start <= end && end <= nodes.size() + 1);
 
     auto tws = nodes[start - 1]->tw;
+    auto *node = nodes[start - 1];
 
     for (size_t step = start; step != end; ++step)
-        tws = TimeWindowSegment::merge(
-            data.durationMatrix(), tws, nodes[step]->tw);
+    {
+        node = n(node);
+        tws = TimeWindowSegment::merge(data.durationMatrix(), tws, node->tw);
+    }
 
     return tws;
 }
 
 Distance Route::distBetween(size_t start, size_t end) const
 {
-    assert(start <= end && end <= nodes.size());
+    assert(start <= end && end <= nodes.size() + 1);
 
     auto const startDist = start == 0 ? 0 : nodes[start - 1]->cumulatedDistance;
-    auto const endDist = nodes[end - 1]->cumulatedDistance;
+    auto const endDist = end == nodes.size() + 1
+                             ? endDepot.cumulatedDistance
+                             : nodes[end - 1]->cumulatedDistance;
 
     assert(startDist <= endDist);
 
     return endDist - startDist;
 }
 
 Load Route::loadBetween(size_t start, size_t end) const
 {
-    assert(start <= end && end <= nodes.size());
+    assert(start <= end && end <= nodes.size() + 1);
 
-    auto const *startNode = start == 0 ? depot : nodes[start - 1];
+    auto const *startNode = start == 0 ? &startDepot : nodes[start - 1];
     auto const atStart = data.client(startNode->client).demand;
     auto const startLoad = startNode->cumulatedLoad;
-    auto const endLoad = nodes[end - 1]->cumulatedLoad;
+    auto const endLoad = end == nodes.size() + 1
+                             ? endDepot.cumulatedLoad
+                             : nodes[end - 1]->cumulatedLoad;
 
     assert(startLoad <= endLoad);
 
     return endLoad - startLoad + atStart;
 }
 }  // namespace pyvrp::search
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/SwapStar.cpp` & `pyvrp-0.5.0/pyvrp/cpp/search/SwapStar.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #include "SwapStar.h"
 
+#include <cassert>
+
 using pyvrp::Cost;
-using pyvrp::search::Node;
+using pyvrp::search::Route;
 using pyvrp::search::SwapStar;
 using TWS = pyvrp::TimeWindowSegment;
 
 void SwapStar::updateRemovalCosts(Route *R1, CostEvaluator const &costEvaluator)
 {
-    for (Node *U = n(R1->depot); !U->isDepot(); U = n(U))
+    for (auto *U : *R1)
     {
         auto twData
             = TWS::merge(data.durationMatrix(), p(U)->twBefore, n(U)->twAfter);
 
         Distance const deltaDist = data.dist(p(U)->client, n(U)->client)
                                    - data.dist(p(U)->client, U->client)
                                    - data.dist(U->client, n(U)->client);
@@ -20,37 +22,40 @@
             = static_cast<Cost>(deltaDist)
               + costEvaluator.twPenalty(twData.totalTimeWarp())
               - costEvaluator.twPenalty(R1->timeWarp());
     }
 }
 
 void SwapStar::updateInsertionCost(Route *R,
-                                   Node *U,
+                                   Route::Node *U,
                                    CostEvaluator const &costEvaluator)
 {
     auto &insertPositions = cache(R->idx, U->client);
 
     insertPositions = {};
     insertPositions.shouldUpdate = false;
 
     // Insert cost of U just after the depot (0 -> U -> ...)
-    auto twData = TWS::merge(
-        data.durationMatrix(), R->depot->twBefore, U->tw, n(R->depot)->twAfter);
-
-    Distance deltaDist = data.dist(0, U->client)
-                         + data.dist(U->client, n(R->depot)->client)
-                         - data.dist(0, n(R->depot)->client);
+    auto twData = TWS::merge(data.durationMatrix(),
+                             R->startDepot.twBefore,
+                             U->tw,
+                             n(&R->startDepot)->twAfter);
+
+    Distance deltaDist
+        = data.dist(R->startDepot.client, U->client)
+          + data.dist(U->client, n(&R->startDepot)->client)
+          - data.dist(R->startDepot.client, n(&R->startDepot)->client);
 
     Cost deltaCost = static_cast<Cost>(deltaDist)
                      + costEvaluator.twPenalty(twData.totalTimeWarp())
                      - costEvaluator.twPenalty(R->timeWarp());
 
-    insertPositions.maybeAdd(deltaCost, R->depot);
+    insertPositions.maybeAdd(deltaCost, &R->startDepot);
 
-    for (Node *V = n(R->depot); !V->isDepot(); V = n(V))
+    for (auto *V : *R)
     {
         // Insert cost of U just after V (V -> U -> ...)
         twData = TWS::merge(
             data.durationMatrix(), V->twBefore, U->tw, n(V)->twAfter);
 
         deltaDist = data.dist(V->client, U->client)
                     + data.dist(U->client, n(V)->client)
@@ -60,16 +65,16 @@
                     + costEvaluator.twPenalty(twData.totalTimeWarp())
                     - costEvaluator.twPenalty(R->timeWarp());
 
         insertPositions.maybeAdd(deltaCost, V);
     }
 }
 
-std::pair<Cost, Node *> SwapStar::getBestInsertPoint(
-    Node *U, Node *V, CostEvaluator const &costEvaluator)
+std::pair<Cost, Route::Node *> SwapStar::getBestInsertPoint(
+    Route::Node *U, Route::Node *V, CostEvaluator const &costEvaluator)
 {
     auto &best_ = cache(V->route->idx, U->client);
 
     if (best_.shouldUpdate)  // then we first update the insert positions
         updateInsertionCost(V->route, U, costEvaluator);
 
     for (size_t idx = 0; idx != 3; ++idx)  // only OK if V is not adjacent
@@ -116,16 +121,16 @@
         updateRemovalCosts(routeU, costEvaluator);
         updated[routeV->idx] = false;
 
         for (size_t idx = 1; idx != data.numClients() + 1; ++idx)
             cache(routeU->idx, idx).shouldUpdate = true;
     }
 
-    for (Node *U = n(routeU->depot); !U->isDepot(); U = n(U))
-        for (Node *V = n(routeV->depot); !V->isDepot(); V = n(V))
+    for (auto *U : *routeU)
+        for (auto *V : *routeV)
         {
             Cost deltaCost = 0;
 
             auto const uDemand = data.client(U->client).demand;
             auto const vDemand = data.client(V->client).demand;
             auto const loadDiff = uDemand - vDemand;
 
@@ -198,16 +203,19 @@
     else
         deltaDist += data.dist(best.U->client, n(best.UAfter)->client)
                      + data.dist(p(best.V)->client, n(best.V)->client)
                      - data.dist(best.UAfter->client, n(best.UAfter)->client);
 
     Cost deltaCost = static_cast<Cost>(deltaDist);
 
-    // It is not possible to have UAfter == V or VAfter == U, so the positions
-    // are always strictly different
+    // We cannot have that UAfter == V or VAfter == U, as the positions must
+    // always be strictly different.
+    assert(best.VAfter->position != best.U->position);
+    assert(best.UAfter->position != best.V->position);
+
     if (best.VAfter->position + 1 == best.U->position)
     {
         // Special case
         auto uTWS = TWS::merge(data.durationMatrix(),
                                best.VAfter->twBefore,
                                best.V->tw,
                                n(best.U)->twAfter);
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/SwapStar.h` & `pyvrp-0.5.0/pyvrp/cpp/search/SwapStar.h`

 * *Files 18% similar despite different names*

```diff
@@ -8,35 +8,40 @@
 #include <array>
 #include <limits>
 #include <vector>
 
 namespace pyvrp::search
 {
 /**
+ * SwapStar()
+ *
  * Explores the SWAP* neighbourhood of [1]. The SWAP* neighbourhood explores
- * free form re-insertions of nodes U and V in the given routes (so the nodes
- * are exchanged between routes, but they are not necessarily inserted in
- * the same place as the other exchanged node). Our implementation of the
- * neighbourhood follows Algorithm 2 of [1] fairly faithfully.
- * <br />
- * Thibaut Vidal. 2022. Hybrid genetic search for the CVRP: Open-source
- * implementation and SWAP* neighborhood. Comput. Oper. Res. 140.
- * https://doi.org/10.1016/j.cor.2021.105643
+ * free form re-insertions of clients :math:`U` and :math:`V` in the given
+ * routes (so the clients are exchanged between routes, but they are not
+ * necessarily inserted in the place of the other exchanged client). Our
+ * implementation of the SWAP* neighbourhood follows Algorithm 2 of [1] fairly
+ * closely.
+ *
+ * References
+ * ----------
+ * .. [1] Thibaut Vidal. 2022. Hybrid genetic search for the CVRP: Open-source
+ *        implementation and SWAP* neighborhood. *Comput. Oper. Res*. 140.
+ *        https://doi.org/10.1016/j.cor.2021.105643
  */
 class SwapStar : public LocalSearchOperator<Route>
 {
     struct ThreeBest  // stores three best SWAP* insertion points
     {
         bool shouldUpdate = true;
         std::array<Cost, 3> costs = {std::numeric_limits<Cost>::max(),
                                      std::numeric_limits<Cost>::max(),
                                      std::numeric_limits<Cost>::max()};
-        std::array<Node *, 3> locs = {nullptr, nullptr, nullptr};
+        std::array<Route::Node *, 3> locs = {nullptr, nullptr, nullptr};
 
-        void maybeAdd(Cost costInsert, Node *placeInsert)
+        void maybeAdd(Cost costInsert, Route::Node *placeInsert)
         {
             if (costInsert >= costs[2])
                 return;
 
             if (costInsert >= costs[1])
             {
                 costs[2] = costInsert;
@@ -61,33 +66,34 @@
         }
     };
 
     struct BestMove  // tracks the best SWAP* move
     {
         Cost cost = 0;
 
-        Node *U = nullptr;
-        Node *UAfter = nullptr;
+        Route::Node *U = nullptr;
+        Route::Node *UAfter = nullptr;
 
-        Node *V = nullptr;
-        Node *VAfter = nullptr;
+        Route::Node *V = nullptr;
+        Route::Node *VAfter = nullptr;
     };
 
     // Updates the removal costs of clients in the given route
     void updateRemovalCosts(Route *R1, CostEvaluator const &costEvaluator);
 
     // Updates the cache storing the three best positions in the given route for
     // the passed-in node (client).
-    void
-    updateInsertionCost(Route *R, Node *U, CostEvaluator const &costEvaluator);
+    void updateInsertionCost(Route *R,
+                             Route::Node *U,
+                             CostEvaluator const &costEvaluator);
 
     // Gets the delta cost and reinsert point for U in the route of V, assuming
     // V is removed.
-    inline std::pair<Cost, Node *>
-    getBestInsertPoint(Node *U, Node *V, CostEvaluator const &costEvaluator);
+    inline std::pair<Cost, Route::Node *> getBestInsertPoint(
+        Route::Node *U, Route::Node *V, CostEvaluator const &costEvaluator);
 
     Matrix<ThreeBest> cache;
     Matrix<Cost> removalCosts;
     std::vector<bool> updated;
 
     BestMove best;
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/TwoOpt.cpp` & `pyvrp-0.5.0/pyvrp/cpp/search/TwoOpt.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -3,27 +3,34 @@
 #include "Route.h"
 #include "TimeWindowSegment.h"
 
 using pyvrp::Cost;
 using pyvrp::search::TwoOpt;
 using TWS = pyvrp::TimeWindowSegment;
 
-Cost TwoOpt::evalWithinRoute(Node *U,
-                             Node *V,
+Cost TwoOpt::evalWithinRoute(Route::Node *U,
+                             Route::Node *V,
                              CostEvaluator const &costEvaluator) const
 {
     if (U->position + 1 >= V->position)
         return 0;
 
-    Distance const deltaDist = data.dist(U->client, V->client)
-                               + data.dist(n(U)->client, n(V)->client)
-                               + V->cumulatedReversalDistance
-                               - data.dist(U->client, n(U)->client)
-                               - data.dist(V->client, n(V)->client)
-                               - n(U)->cumulatedReversalDistance;
+    // Current situation is U -> n(U) -> ... -> V -> n(V). Proposed move is
+    // U -> V -> p(V) -> ... -> n(U) -> n(V). This reverses the segment from
+    // n(U) to V.
+    Distance segmentReversalDistance = 0;  // reversal dist of n(U) -> ... -> V
+    for (auto *node = V; node != n(U); node = p(node))
+        segmentReversalDistance += data.dist(node->client, p(node)->client);
+
+    Distance const deltaDist
+        = data.dist(U->client, V->client)
+          + data.dist(n(U)->client, n(V)->client) + segmentReversalDistance
+          - data.dist(U->client, n(U)->client)
+          - data.dist(V->client, n(V)->client)
+          - U->route->distBetween(n(U)->position, V->position);
 
     Cost deltaCost = static_cast<Cost>(deltaDist);
 
     if (!U->route->hasTimeWarp() && deltaCost >= 0)
         return deltaCost;
 
     auto tws = U->twBefore;
@@ -38,16 +45,16 @@
 
     deltaCost += costEvaluator.twPenalty(tws.totalTimeWarp());
     deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
 
     return deltaCost;
 }
 
-Cost TwoOpt::evalBetweenRoutes(Node *U,
-                               Node *V,
+Cost TwoOpt::evalBetweenRoutes(Route::Node *U,
+                               Route::Node *V,
                                CostEvaluator const &costEvaluator) const
 {
     Distance const current = data.dist(U->client, n(U)->client)
                              + data.dist(V->client, n(V)->client);
     Distance const proposed = data.dist(U->client, n(V)->client)
                               + data.dist(V->client, n(U)->client);
 
@@ -79,30 +86,30 @@
                                            V->route->capacity());
     deltaCost
         -= costEvaluator.loadPenalty(V->route->load(), V->route->capacity());
 
     return deltaCost;
 }
 
-void TwoOpt::applyWithinRoute(Node *U, Node *V) const
+void TwoOpt::applyWithinRoute(Route::Node *U, Route::Node *V) const
 {
     auto *itRoute = V;
     auto *insertionPoint = U;
     auto *currNext = n(U);
 
-    while (itRoute != currNext)  // No need to move x, we pivot around it
+    while (itRoute != currNext)  // No need to move n(U), we pivot around it
     {
         auto *current = itRoute;
         itRoute = p(itRoute);
         current->insertAfter(insertionPoint);
         insertionPoint = current;
     }
 }
 
-void TwoOpt::applyBetweenRoutes(Node *U, Node *V) const
+void TwoOpt::applyBetweenRoutes(Route::Node *U, Route::Node *V) const
 {
     auto *itRouteU = n(U);
     auto *itRouteV = n(V);
 
     auto *insertLocation = U;
     while (!itRouteV->isDepot())
     {
@@ -118,23 +125,25 @@
         auto *node = itRouteU;
         itRouteU = n(itRouteU);
         node->insertAfter(insertLocation);
         insertLocation = node;
     }
 }
 
-Cost TwoOpt::evaluate(Node *U, Node *V, CostEvaluator const &costEvaluator)
+Cost TwoOpt::evaluate(Route::Node *U,
+                      Route::Node *V,
+                      CostEvaluator const &costEvaluator)
 {
     if (U->route->idx > V->route->idx)  // will be tackled in a later iteration
         return 0;                       // - no need to process here already
 
     return U->route == V->route ? evalWithinRoute(U, V, costEvaluator)
                                 : evalBetweenRoutes(U, V, costEvaluator);
 }
 
-void TwoOpt::apply(Node *U, Node *V) const
+void TwoOpt::apply(Route::Node *U, Route::Node *V) const
 {
     if (U->route == V->route)
         applyWithinRoute(U, V);
     else
         applyBetweenRoutes(U, V);
 }
```

### Comparing `pyvrp-0.4.4/pyvrp/cpp/search/bindings.cpp` & `pyvrp-0.5.0/pyvrp/cpp/search/bindings.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #include "Exchange.h"
 #include "LocalSearch.h"
 #include "MoveTwoClientsReversed.h"
 #include "RelocateStar.h"
 #include "SwapStar.h"
 #include "TwoOpt.h"
+#include "search_docs.h"
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 
 namespace py = pybind11;
 
 using pyvrp::search::Exchange;
@@ -16,73 +17,73 @@
 using pyvrp::search::MoveTwoClientsReversed;
 using pyvrp::search::RelocateStar;
 using pyvrp::search::SwapStar;
 using pyvrp::search::TwoOpt;
 
 PYBIND11_MODULE(_search, m)
 {
-    using NodeOp = LocalSearchOperator<pyvrp::search::Node>;
+    using NodeOp = LocalSearchOperator<pyvrp::search::Route::Node>;
     using RouteOp = LocalSearchOperator<pyvrp::search::Route>;
 
     py::class_<NodeOp>(m, "NodeOperator");
     py::class_<RouteOp>(m, "RouteOperator");
 
-    py::class_<Exchange<1, 0>, NodeOp>(m, "Exchange10")
+    py::class_<Exchange<1, 0>, NodeOp>(
+        m, "Exchange10", DOC(pyvrp, search, Exchange))
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
-             py::keep_alive<1, 2>()  // keep data alive
-        );
+             py::keep_alive<1, 2>());  // keep data alive
 
-    py::class_<Exchange<2, 0>, NodeOp>(m, "Exchange20")
+    py::class_<Exchange<2, 0>, NodeOp>(
+        m, "Exchange20", DOC(pyvrp, search, Exchange))
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
-             py::keep_alive<1, 2>()  // keep data alive
-        );
+             py::keep_alive<1, 2>());  // keep data alive
 
-    py::class_<Exchange<3, 0>, NodeOp>(m, "Exchange30")
+    py::class_<Exchange<3, 0>, NodeOp>(
+        m, "Exchange30", DOC(pyvrp, search, Exchange))
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
-             py::keep_alive<1, 2>()  // keep data alive
-        );
+             py::keep_alive<1, 2>());  // keep data alive
 
-    py::class_<Exchange<1, 1>, NodeOp>(m, "Exchange11")
+    py::class_<Exchange<1, 1>, NodeOp>(
+        m, "Exchange11", DOC(pyvrp, search, Exchange))
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
-             py::keep_alive<1, 2>()  // keep data alive
-        );
+             py::keep_alive<1, 2>());  // keep data alive
 
-    py::class_<Exchange<2, 1>, NodeOp>(m, "Exchange21")
+    py::class_<Exchange<2, 1>, NodeOp>(
+        m, "Exchange21", DOC(pyvrp, search, Exchange))
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
-             py::keep_alive<1, 2>()  // keep data alive
-        );
+             py::keep_alive<1, 2>());  // keep data alive
 
-    py::class_<Exchange<3, 1>, NodeOp>(m, "Exchange31")
+    py::class_<Exchange<3, 1>, NodeOp>(
+        m, "Exchange31", DOC(pyvrp, search, Exchange))
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
-             py::keep_alive<1, 2>()  // keep data alive
-        );
+             py::keep_alive<1, 2>());  // keep data alive
 
-    py::class_<Exchange<2, 2>, NodeOp>(m, "Exchange22")
+    py::class_<Exchange<2, 2>, NodeOp>(
+        m, "Exchange22", DOC(pyvrp, search, Exchange))
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
-             py::keep_alive<1, 2>()  // keep data alive
-        );
+             py::keep_alive<1, 2>());  // keep data alive
 
-    py::class_<Exchange<3, 2>, NodeOp>(m, "Exchange32")
+    py::class_<Exchange<3, 2>, NodeOp>(
+        m, "Exchange32", DOC(pyvrp, search, Exchange))
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
-             py::keep_alive<1, 2>()  // keep data alive
-        );
+             py::keep_alive<1, 2>());  // keep data alive
 
-    py::class_<Exchange<3, 3>, NodeOp>(m, "Exchange33")
+    py::class_<Exchange<3, 3>, NodeOp>(
+        m, "Exchange33", DOC(pyvrp, search, Exchange))
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
-             py::keep_alive<1, 2>()  // keep data alive
-        );
+             py::keep_alive<1, 2>());  // keep data alive
 
     py::class_<LocalSearch>(m, "LocalSearch")
         .def(py::init<pyvrp::ProblemData const &,
                       std::vector<std::vector<int>>>(),
              py::arg("data"),
              py::arg("neighbours"),
              py::keep_alive<1, 2>())  // keep data alive until LS is freed
@@ -96,38 +97,46 @@
              py::keep_alive<1, 2>())
         .def("set_neighbours",
              &LocalSearch::setNeighbours,
              py::arg("neighbours"))
         .def("get_neighbours",
              &LocalSearch::getNeighbours,
              py::return_value_policy::reference_internal)
+        .def("__call__",
+             &LocalSearch::operator(),
+             py::arg("solution"),
+             py::arg("cost_evaluator"))
         .def("search",
-             &LocalSearch::search,
+             py::overload_cast<pyvrp::Solution const &,
+                               pyvrp::CostEvaluator const &>(
+                 &LocalSearch::search),
              py::arg("solution"),
              py::arg("cost_evaluator"))
         .def("intensify",
-             &LocalSearch::intensify,
+             py::overload_cast<pyvrp::Solution const &,
+                               pyvrp::CostEvaluator const &,
+                               double const>(&LocalSearch::intensify),
              py::arg("solution"),
              py::arg("cost_evaluator"),
-             py::arg("overlap_tolerance_degrees") = 0)
+             py::arg("overlap_tolerance") = 0.05)
         .def("shuffle", &LocalSearch::shuffle, py::arg("rng"));
 
     py::class_<MoveTwoClientsReversed, NodeOp>(m, "MoveTwoClientsReversed")
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
              py::keep_alive<1, 2>()  // keep data alive
         );
 
     py::class_<RelocateStar, RouteOp>(m, "RelocateStar")
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
              py::keep_alive<1, 2>()  // keep data alive
         );
 
-    py::class_<SwapStar, RouteOp>(m, "SwapStar")
+    py::class_<SwapStar, RouteOp>(m, "SwapStar", DOC(pyvrp, search, SwapStar))
         .def(py::init<pyvrp::ProblemData const &>(),
              py::arg("data"),
              py::keep_alive<1, 2>()  // keep data alive
         );
 
     py::class_<TwoOpt, NodeOp>(m, "TwoOpt")
         .def(py::init<pyvrp::ProblemData const &>(),
```

### Comparing `pyvrp-0.4.4/pyvrp/crossover/selective_route_exchange.py` & `pyvrp-0.5.0/pyvrp/crossover/selective_route_exchange.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from typing import Tuple
 
-from pyvrp._pyvrp import CostEvaluator, ProblemData, Solution, XorShift128
+from pyvrp._pyvrp import (
+    CostEvaluator,
+    ProblemData,
+    RandomNumberGenerator,
+    Solution,
+)
 
 from ._crossover import selective_route_exchange as _srex
 
 
 def selective_route_exchange(
     parents: Tuple[Solution, Solution],
     data: ProblemData,
     cost_evaluator: CostEvaluator,
-    rng: XorShift128,
+    rng: RandomNumberGenerator,
 ) -> Solution:
     """
     This crossover operator due to Nagata and Kobayashi (2010) combines routes
     from both parents to generate a new offspring solution. It does this by
     carefully selecting routes from the second parent that could be exchanged
     with routes from the first parent. After exchanging these routes, the
     resulting offspring solution is repaired using a greedy repair strategy.
```

### Comparing `pyvrp-0.4.4/pyvrp/crossover/tests/test_selective_route_exchange.py` & `pyvrp-0.5.0/pyvrp/crossover/tests/test_selective_route_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import itertools
 
 from numpy.testing import assert_equal, assert_raises
 from pytest import mark
 
-from pyvrp import CostEvaluator, Route, Solution, VehicleType, XorShift128
+from pyvrp import (
+    CostEvaluator,
+    RandomNumberGenerator,
+    Route,
+    Solution,
+    VehicleType,
+)
 from pyvrp.crossover import selective_route_exchange as srex
 from pyvrp.crossover._crossover import selective_route_exchange as cpp_srex
 from pyvrp.tests.helpers import make_heterogeneous, read
 
 
 def test_same_parents_same_offspring():
     """
     Tests that SREX produces identical offspring when both parents are the
     same.
     """
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     solution = Solution(data, [[1, 2], [3, 4]])
     offspring = srex((solution, solution), data, cost_evaluator, rng)
 
     assert_equal(offspring, solution)
 
 
 def test_srex_empty_solution():
     data = read("data/p06-2-50.vrp", round_func="dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     empty = Solution(data, [])
     nonempty = Solution(data, [[1, 2, 3, 4]])
 
     # If both parents are empty the returned offspring must also be empty.
     offspring = srex((empty, empty), data, cost_evaluator, rng)
     assert_equal(offspring, empty)
@@ -40,15 +46,15 @@
     # solution is the nonempty parent.
     for parents in [(empty, nonempty), (nonempty, empty)]:
         offspring = srex(parents, data, cost_evaluator, rng)
         assert_equal(offspring, nonempty)
 
 
 @mark.parametrize(
-    "idx1, idx2, num_moved_routes",
+    ("idx1", "idx2", "num_moved_routes"),
     [
         (10, 0, 1),  # idx1 >= # routes first
         (0, 10, 1),  # idx2 >= # routes second
         (0, 0, 0),  # num_moved_routes < 1
         (0, 0, 2),  # num_moved_routes > min(# routes first, # routes second)
     ],
 )
```

### Comparing `pyvrp-0.4.4/pyvrp/diversity/_diversity.pyi` & `pyvrp-0.5.0/pyvrp/cpp/diversity/diversity.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,55 @@
-from pyvrp._pyvrp import Solution
+#ifndef PYVRP_DIVERSITY_H
+#define PYVRP_DIVERSITY_H
 
-def broken_pairs_distance(first: Solution, second: Solution) -> float:
-    """
-    Computes the symmetric broken pairs distance (BPD) between the given two
-    solutions. This function determines whether each client in the problem
-    shares neighbours between the first and second solution. If not, the
-    client is part of a 'broken pair': a link that is part of one solution,
-    but not of the other.
+#include "ProblemData.h"
+#include "Solution.h"
 
-    Formally, given two solutions :math:`f` and :math:`s`, let :math:`p_f(i)`
-    and :math:`p_s(i)` be the preceding client (or depot) of client
-    :math:`i = 1, \\ldots, n` in :math:`f` and :math:`s`, respectively.
-    Similarly define :math:`s_f(i)` and :math:`s_s(i)` for the succeeding
-    client (or depot). Then, we have
+#include <functional>
 
-    .. math::
+namespace pyvrp::diversity
+{
+typedef std::function<double(Solution const &, Solution const &)>
+    DiversityMeasure;
+
+/**
+ * Computes the symmetric broken pairs distance (BPD) between the given two
+ * solutions. This function determines whether each client in the problem
+ * shares neighbours between the first and second solution. If not, the
+ * client is part of a 'broken pair': a link that is part of one solution,
+ * but not of the other.
+ *
+ * Formally, given two solutions :math:`f` and :math:`s`, let :math:`p_f(i)`
+ * and :math:`p_s(i)` be the preceding client (or depot) of client
+ * :math:`i = 1, \ldots, n` in :math:`f` and :math:`s`, respectively.
+ * Similarly define :math:`s_f(i)` and :math:`s_s(i)` for the succeeding
+ * client (or depot). Then, we have
+ *
+ * .. math::
+ *
+ *    \text{BPD}(f, s) = \frac{
+ *        \sum_{i = 1}^n 1_{p_f(i) \ne p_s(i)} + 1_{s_f(i) \ne s_s(i)}
+ *    }{2n}.
+ *
+ * .. note::
+ *
+ *    Note that our definition is directed: a route ``[1, 2, 3, 4]`` is
+ *    considered completely different from a route ``[4, 3, 2, 1]``.
+ *
+ * Parameters
+ * ----------
+ * first
+ *     First solution.
+ * second
+ *     Second solution.
+ *
+ * Returns
+ * -------
+ * float
+ *     A value in [0, 1] that indicates the percentage of broken links between
+ *     the two solutions. A value near one suggests the solutions are
+ *     maximally diverse, a value of zero indicates they are the same.
+ */
+double brokenPairsDistance(Solution const &first, Solution const &second);
+}  // namespace pyvrp::diversity
 
-       \\text{BPD}(f, s) = \\frac{
-            \\sum_{i = 1}^n 1_{p_f(i) \\ne p_s(i)} + 1_{s_f(i) \\ne s_s(i)}
-        }{2n}.
-
-    .. note::
-
-        Note that our definition is directed: a route ``[1, 2, 3, 4]`` is
-        considered completely different from a route ``[4, 3, 2, 1]``.
-
-    Parameters
-    ----------
-    first
-        First solution.
-    second
-        Second solution.
-
-    Returns
-    -------
-    float
-        A value in [0, 1] that indicates the percentage of broken links between
-        the two solutions. A value near one suggests the solutions are
-        maximally diverse, a value of zero indicates they are the same.
-    """
+#endif  // PYVRP_DIVERSITY_H
```

### Comparing `pyvrp-0.4.4/pyvrp/diversity/tests/test_broken_pairs_distance.py` & `pyvrp-0.5.0/pyvrp/diversity/tests/test_broken_pairs_distance.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/plotting/plot_coordinates.py` & `pyvrp-0.5.0/pyvrp/plotting/plot_coordinates.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/plotting/plot_demands.py` & `pyvrp-0.5.0/pyvrp/plotting/plot_demands.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/plotting/plot_diversity.py` & `pyvrp-0.5.0/pyvrp/plotting/plot_diversity.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 from typing import Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from pyvrp.Result import Result
-from pyvrp.exceptions import StatisticsNotCollectedError
 
 
 def plot_diversity(result: Result, ax: Optional[plt.Axes] = None):
     """
     Plots population diversity statistics.
 
     Parameters
     ----------
     result
         Result for which to plot diversity.
     ax, optional
         Axes object to draw the plot on. One will be created if not
         provided.
-
-    Raises
-    ------
-    StatisticsNotCollectedError
-        Raised when statistics have not been collected.
     """
-    if not result.has_statistics():
-        raise StatisticsNotCollectedError(
-            "Statistics have not been collected."
-        )
-
     if not ax:
         _, ax = plt.subplots()
 
     ax.set_title("Diversity")
     ax.set_xlabel("Iteration (#)")
     ax.set_ylabel("Avg. diversity")
```

### Comparing `pyvrp-0.4.4/pyvrp/plotting/plot_instance.py` & `pyvrp-0.5.0/pyvrp/plotting/plot_instance.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/plotting/plot_objectives.py` & `pyvrp-0.5.0/pyvrp/plotting/plot_objectives.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Optional, Tuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from pyvrp.Result import Result
-from pyvrp.exceptions import StatisticsNotCollectedError
 
 
 def plot_objectives(
     result: Result,
     num_to_skip: Optional[int] = None,
     ax: Optional[plt.Axes] = None,
     ylim_adjust: Tuple[float, float] = (0.95, 1.15),
@@ -26,25 +25,15 @@
         later in the search. The default skips the first 5% of iterations.
     ax
         Axes object to draw the plot on. One will be created if not provided.
     ylim_adjust
         Bounds the y-axis to ``(best * ylim_adjust[0], best * ylim_adjust[1])``
         where ``best`` denotes the best found feasible objective value. Default
         (0.95, 1.15).
-
-    Raises
-    ------
-    StatisticsNotCollectedError
-        Raised when statistics have not been collected.
     """
-    if not result.has_statistics():
-        raise StatisticsNotCollectedError(
-            "Statistics have not been collected."
-        )
-
     if not ax:
         _, ax = plt.subplots()
 
     if num_to_skip is None:
         num_to_skip = int(0.05 * result.num_iterations)
 
     def _plot(x, y, *args, **kwargs):
```

### Comparing `pyvrp-0.4.4/pyvrp/plotting/plot_result.py` & `pyvrp-0.5.0/pyvrp/plotting/plot_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def plot_result(
     result: Result, data: ProblemData, fig: Optional[plt.Figure] = None
 ):
     """
     Plots the results of a run, including the best solution and detailed
-    statistics about the algorithm's performance (if available).
+    statistics about the algorithm's performance.
 
     Parameters
     ----------
     result
         Result to be plotted.
     data
         Data instance underlying the result's solution.
@@ -34,14 +34,13 @@
     # two columns: left and right. Left has three rows, each containing a
     # plot with statistics: the first plots population diversity, the
     # second subpopulation objective information, and the third iteration
     # runtimes. The right column plots the solution on top of the instance
     # data.
     gs = fig.add_gridspec(3, 2, width_ratios=(2 / 5, 3 / 5))
 
-    if result.has_statistics():
-        ax_div = fig.add_subplot(gs[0, 0])
-        plot_diversity(result, ax=ax_div)
-        plot_objectives(result, ax=fig.add_subplot(gs[1, 0], sharex=ax_div))
-        plot_runtimes(result, ax=fig.add_subplot(gs[2, 0], sharex=ax_div))
+    ax_div = fig.add_subplot(gs[0, 0])
+    plot_diversity(result, ax=ax_div)
+    plot_objectives(result, ax=fig.add_subplot(gs[1, 0], sharex=ax_div))
+    plot_runtimes(result, ax=fig.add_subplot(gs[2, 0], sharex=ax_div))
 
     plot_solution(result.best, data, ax=fig.add_subplot(gs[:, 1]))
```

### Comparing `pyvrp-0.4.4/pyvrp/plotting/plot_route_schedule.py` & `pyvrp-0.5.0/pyvrp/plotting/plot_route_schedule.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     route: Route,
     legend: bool = True,
     title: Optional[str] = None,
     ax: Optional[plt.Axes] = None,
 ):
     """
     Plots a route schedule. This function plots multiple time statistics
-    as a function of distance traveled:
+    as a function of distance travelled:
 
     * Solid: earliest possible trajectory / time, using time warp if the route
       is infeasible.
     * Shaded: slack up to latest possible trajectory / time, only if no time
       warp on the route.
     * Dash-dotted: driving and service time, excluding wait time and time warp.
     * Dotted: pure driving time.
@@ -39,15 +39,15 @@
     ax, optional
         Axes object to draw the plot on. One will be created if not provided.
     """
     if not ax:
         _, ax = plt.subplots()
 
     vehicle_type = data.vehicle_type(route.vehicle_type())
-    depot = data.client(0)  # For readability, define variable
+    depot = data.client(vehicle_type.depot)
     horizon = depot.tw_late - depot.tw_early
 
     # Initialise tracking variables
     t = route.release_time()
     drive_time = 0
     serv_time = 0
     dist = 0
@@ -71,16 +71,16 @@
     add_traces(dist, t, drive_time, serv_time, load)
 
     t += depot.service_duration
     serv_time += depot.service_duration
 
     add_traces(dist, t, drive_time, serv_time, load)
 
-    prev_idx = 0  # depot
-    for idx in list(route) + [0]:
+    prev_idx = vehicle_type.depot
+    for idx in [*list(route), vehicle_type.depot]:
         stop = data.client(idx)
         delta_time = data.duration(prev_idx, idx)
         delta_dist = data.dist(prev_idx, idx)
         t += delta_time
         drive_time += delta_time
         dist += delta_dist
 
@@ -94,15 +94,15 @@
             timewarp_lines.append(((dist, t), (dist, stop.tw_late)))
             t = stop.tw_late
 
         load -= stop.demand
 
         add_traces(dist, t, drive_time, serv_time, load)
 
-        if idx != 0:  # Don't plot service and timewindow for return to depot
+        if idx != vehicle_type.depot:  # exclude return to depot
             t += stop.service_duration
             serv_time += stop.service_duration
 
             add_traces(dist, t, drive_time, serv_time, load)
 
             timewindow_lines.append(
                 ((dist, stop.tw_early), (dist, stop.tw_late))
```

### Comparing `pyvrp-0.4.4/pyvrp/plotting/plot_solution.py` & `pyvrp-0.5.0/pyvrp/plotting/plot_solution.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 from pyvrp import ProblemData, Solution
 
 
 def plot_solution(
     solution: Solution,
     data: ProblemData,
-    plot_customers: bool = False,
+    plot_clients: bool = False,
     ax: Optional[plt.Axes] = None,
 ):
     """
     Plots the given solution.
 
     Parameters
     ----------
     solution
         Solution to plot.
     data
         Data instance underlying the solution.
-    plot_customers, optional
-        Whether to plot customers as dots. Default False, which plots only the
+    plot_clients, optional
+        Whether to plot clients as dots. Default False, which plots only the
         solution's routes.
     ax, optional
         Axes object to draw the plot on. One will be created if not provided.
     """
     if not ax:
         _, ax = plt.subplots()
 
@@ -38,16 +38,16 @@
     kwargs = dict(c="tab:red", marker="*", zorder=3, s=500)
     ax.scatter(x_coords[0], y_coords[0], label="Depot", **kwargs)
 
     for idx, route in enumerate(solution.get_routes(), 1):
         x = x_coords[route]
         y = y_coords[route]
 
-        # Coordinates of customers served by this route.
-        if len(route) == 1 or plot_customers:
+        # Coordinates of clients served by this route.
+        if len(route) == 1 or plot_clients:
             ax.scatter(x, y, label=f"Route {idx}", zorder=3, s=75)
         ax.plot(x, y)
 
         # Edges from and to the depot, very thinly dashed.
         kwargs = dict(ls=(0, (5, 15)), linewidth=0.25, color="grey")
         ax.plot([x_coords[0], x[0]], [y_coords[0], y[0]], **kwargs)
         ax.plot([x[-1], x_coords[0]], [y[-1], y_coords[0]], **kwargs)
```

### Comparing `pyvrp-0.4.4/pyvrp/plotting/plot_time_windows.py` & `pyvrp-0.5.0/pyvrp/plotting/plot_time_windows.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png` & `pyvrp-0.5.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png` & `pyvrp-0.5.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png` & `pyvrp-0.5.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png` & `pyvrp-0.5.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png` & `pyvrp-0.5.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/plotting/tests/test_plotting.py` & `pyvrp-0.5.0/pyvrp/tests/test_Result.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,84 @@
-from matplotlib.testing.decorators import image_comparison as img_comp
-from numpy.testing import assert_, assert_raises
+import math
 
-from pyvrp import (
-    CostEvaluator,
-    Population,
-    PopulationParams,
-    Solution,
-    XorShift128,
-    plotting,
-)
+from numpy.testing import assert_, assert_allclose, assert_equal, assert_raises
+from pytest import mark
+
+from pyvrp import CostEvaluator, Population, RandomNumberGenerator, Solution
 from pyvrp.Result import Result
 from pyvrp.Statistics import Statistics
 from pyvrp.diversity import broken_pairs_distance
-from pyvrp.exceptions import StatisticsNotCollectedError
-from pyvrp.tests.helpers import make_random_solutions, read, read_solution
+from pyvrp.tests.helpers import read
 
-IMG_KWARGS = dict(remove_text=True, tol=2, extensions=["png"], style="mpl20")
 
-
-def test_plotting_methods_raise_when_no_stats_available():
+@mark.parametrize(
+    ("routes", "num_iterations", "runtime"),
+    [([[1, 2], [3], [4]], 1, 1.5), ([[1, 2, 3, 4]], 100, 54.2)],
+)
+def test_fields_are_correctly_set(routes, num_iterations, runtime):
     data = read("data/OkSmall.txt")
-    sol = Solution(data, [[1, 2, 3, 4]])
-    res = Result(sol, Statistics(), 0, 0.0)
-
-    assert_(not res.has_statistics())
-
-    with assert_raises(StatisticsNotCollectedError):
-        plotting.plot_diversity(res)
-
-    with assert_raises(StatisticsNotCollectedError):
-        plotting.plot_objectives(res)
-
-    with assert_raises(StatisticsNotCollectedError):
-        plotting.plot_runtimes(res)
-
-    # These should not raise, since they do not depend on statistics
-    # (plot_solution) or optionally print statistics (plot_result).
-    plotting.plot_solution(res.best, data)
-    plotting.plot_result(res, data)
-
-
-@img_comp(["plot_solution", "plot_solution_with_customers"], **IMG_KWARGS)
-def test_plot_solution():
-    data = read("data/RC208.txt", "solomon", round_func="trunc")
-    bks = read_solution("data/RC208.sol")
+    sol = Solution(data, routes)
 
-    sol = Solution(data, bks)
+    res = Result(sol, Statistics(), num_iterations, runtime)
 
-    plotting.plot_solution(sol, data)
-    plotting.plot_solution(sol, data, plot_customers=True)
+    assert_equal(res.is_feasible(), sol.is_feasible())
+    assert_equal(res.num_iterations, num_iterations)
+    assert_allclose(res.runtime, runtime)
+
+    if sol.is_feasible():
+        assert_allclose(res.cost(), CostEvaluator().cost(sol))
+    else:
+        assert_equal(res.cost(), math.inf)
+
+
+@mark.parametrize(
+    ("num_iterations", "runtime"),
+    [
+        (-1, 0.0),  # num_iterations < 0
+        (0, -1.0),  # runtime < 0
+    ],
+)
+def test_init_raises_invalid_arguments(num_iterations, runtime):
+    data = read("data/OkSmall.txt")
+    sol = Solution(data, [[1, 2, 3, 4]])
 
+    with assert_raises(ValueError):
+        Result(sol, Statistics(), num_iterations, runtime)
 
-@img_comp(["plot_result"], **IMG_KWARGS)
-def test_plot_result():
-    num_iterations = 100
 
-    data = read("data/RC208.txt", "solomon", round_func="trunc")
-    bks = read_solution("data/RC208.sol")
+@mark.parametrize("num_iterations", [0, 1, 10])
+def test_num_iterations(num_iterations: int):
+    data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
-
-    params = PopulationParams()
-    pop = Population(broken_pairs_distance, params=params)
-
-    for sol in make_random_solutions(params.min_pop_size, data, rng):
-        pop.add(sol, cost_evaluator)
-
+    rng = RandomNumberGenerator(seed=42)
+    pop = Population(broken_pairs_distance)
     stats = Statistics()
 
-    for i in range(num_iterations):
-        if i == num_iterations // 2:
-            # Make sure we insert a feasible solution
-            sol = Solution(data, bks)
-        else:
-            sol = Solution.make_random(data, rng)
-
-        pop.add(sol, cost_evaluator)
+    for _ in range(num_iterations):
         stats.collect_from(pop, cost_evaluator)
 
-        # Hacky to produce deterministic result
-        stats.runtimes[-1] = i % 3
-
-    res = Result(Solution(data, bks), stats, num_iterations, 0.0)
-    plotting.plot_result(res, data)
+    best = Solution.make_random(data, rng)
+    res = Result(best, stats, num_iterations, 0.0)
+    assert_equal(res.num_iterations, num_iterations)
 
 
-@img_comp(["plot_instance"], **IMG_KWARGS)
-def test_plot_instance():
-    data = read("data/RC208.txt", "solomon", round_func="trunc")
-    plotting.plot_instance(data)
+@mark.parametrize(
+    "routes",
+    [[[1, 2], [3], [4]], [[1, 2, 3, 4]]],
+)
+def test_str_contains_essential_information(routes):
+    data = read("data/OkSmall.txt")
 
+    sol = Solution(data, routes)
+    res = Result(sol, Statistics(), 0, 0.0)
+    str_representation = str(res)
 
-@img_comp(["plot_route_schedule"], **IMG_KWARGS)
-def test_plot_route_schedule():
-    data = read("data/RC208.txt", "solomon", round_func="trunc")
-    bks = read_solution("data/RC208.sol")
-    sol = Solution(data, bks)
-    plotting.plot_route_schedule(data, sol.get_routes()[0])
+    # Test that feasibility status and solution cost are presented.
+    if sol.is_feasible():
+        cost = CostEvaluator().cost(sol)
+        assert_(str(cost) in str_representation)
+    else:
+        assert_("INFEASIBLE" in str_representation)
+
+    # And make sure that all routes are printed as well.
+    for route in sol.get_routes():
+        assert_(str(route) in str_representation)
```

### Comparing `pyvrp-0.4.4/pyvrp/read.py` & `pyvrp-0.5.0/pyvrp/read.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,24 +67,32 @@
 
             * ``'round'`` rounds the values to the nearest integer;
             * ``'trunc'`` truncates the values to be integral;
             * ``'trunc1'`` or ``'dimacs'`` scale and truncate to the nearest
               decimal;
             * ``'none'`` does no rounding. This is the default.
 
+    Raises
+    ------
+    TypeError
+        When ``round_func`` does not name a rounding function, or is not
+        callable.
+    ValueError
+        When the data file does not provide information on the problem size.
+
     Returns
     -------
     ProblemData
         Data instance constructed from the read data.
     """
     if (key := str(round_func)) in ROUND_FUNCS:
         round_func = ROUND_FUNCS[key]
 
     if not callable(round_func):
-        raise ValueError(
+        raise TypeError(
             f"round_func = {round_func} is not understood. Can be a function,"
             f" or one of {ROUND_FUNCS.keys()}."
         )
 
     instance = vrplib.read_instance(where, instance_format=instance_format)
 
     # A priori checks
@@ -144,29 +152,14 @@
     # Checks
     if len(depots) != 1 or depots[0] != 0:
         raise ValueError(
             "Source file should contain single depot with index 1 "
             + "(depot index should be 0 after subtracting offset 1)"
         )
 
-    if demands[0] != 0:
-        raise ValueError("Demand of depot must be 0")
-
-    if time_windows[0, 0] != 0:
-        raise ValueError("Depot start of time window must be 0")
-
-    if service_times[0] != 0:
-        raise ValueError("Depot service duration must be 0")
-
-    if release_times[0] != 0:
-        raise ValueError("Depot release time must be 0")
-
-    if (time_windows[:, 0] > time_windows[:, 1]).any():
-        raise ValueError("Time window cannot start after end")
-
     clients = [
         Client(
             coords[idx][0],  # x
             coords[idx][1],  # y
             demands[idx],
             service_times[idx],
             time_windows[idx][0],  # TW early
```

### Comparing `pyvrp-0.4.4/pyvrp/search/LocalSearch.py` & `pyvrp-0.5.0/pyvrp/search/LocalSearch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pyvrp import CostEvaluator, ProblemData, Solution, XorShift128
+from pyvrp import CostEvaluator, ProblemData, RandomNumberGenerator, Solution
 
 from ._search import LocalSearch as _LocalSearch
 from ._search import NodeOperator, RouteOperator
 
 
 class LocalSearch:
     """
@@ -19,15 +19,18 @@
     rng
         Random number generator.
     neighbours
         List of lists that defines the local search neighbourhood.
     """
 
     def __init__(
-        self, data: ProblemData, rng: XorShift128, neighbours: List[List[int]]
+        self,
+        data: ProblemData,
+        rng: RandomNumberGenerator,
+        neighbours: List[List[int]],
     ):
         self._ls = _LocalSearch(data, neighbours)
         self._rng = rng
 
     def add_node_operator(self, op: NodeOperator):
         """
         Adds a node operator to this local search object. The node operator
@@ -72,107 +75,76 @@
         Returns
         -------
         list
             The current granular neighbourhood.
         """
         return self._ls.get_neighbours()
 
-    def run(
+    def __call__(
         self,
         solution: Solution,
         cost_evaluator: CostEvaluator,
-        should_intensify: bool,
     ) -> Solution:
         """
         This method uses the :meth:`~search` and :meth:`~intensify` methods to
         iteratively improve the given solution. First, :meth:`~search` is
-        applied. Thereafter, if ``should_intensify`` is true,
-        :meth:`~intensify` is applied. This process repeats until no further
-        improvements are found. Finally, the improved solution is returned.
+        applied. Thereafter, :meth:`~intensify` is applied. This repeats until
+        no further improvements are found. Finally, the improved solution is
+        returned.
 
         Parameters
         ----------
         solution
             The solution to improve through local search.
         cost_evaluator
             Cost evaluator to use.
-        should_intensify
-            Whether to apply :meth:`~intensify`. Intensification can provide
-            much better solutions, but is computationally demanding. By default
-            intensification is applied.
 
         Returns
         -------
         Solution
             The improved solution. This is not the same object as the
             solution that was passed in.
         """
-        # HACK We keep searching and intensifying to mimic the local search
-        # implementation of HGS-CVRP and HGS-VRPTW
-        # TODO separate load/export solution from c++ implementation
-        # so we only need to do it once
-        while True:
-            solution = self.search(solution, cost_evaluator)
-
-            if not should_intensify:
-                return solution
-
-            new_solution = self.intensify(solution, cost_evaluator)
-
-            current_cost = cost_evaluator.penalised_cost(solution)
-            new_cost = cost_evaluator.penalised_cost(new_solution)
-
-            if new_cost < current_cost:
-                solution = new_solution
-                continue
-
-            return solution
+        self._ls.shuffle(self._rng)
+        return self._ls(solution, cost_evaluator)
 
     def intensify(
         self,
         solution: Solution,
         cost_evaluator: CostEvaluator,
-        overlap_tolerance_degrees: int = 0,
+        overlap_tolerance: float = 0.05,
     ) -> Solution:
         """
         This method uses the intensifying route operators on this local search
-        object to improve the given solution. To limit the computation
-        demands of intensification, the  ``overlap_tolerance_degrees`` argument
+        object to improve the given solution. To limit the computational
+        demands of intensification, the  ``overlap_tolerance`` argument
         can be used to limit the number of route pairs that are evaluated.
 
         Parameters
         ----------
         solution
             The solution to improve.
         cost_evaluator
             Cost evaluator to use.
-        overlap_tolerance_degrees
+        overlap_tolerance
             This method evaluates improving moves between route pairs. To limit
             computational efforts, by default not all route pairs are
             considered: only those route pairs that share some overlap when
-            considering their center's angle from the depot are evaluted.
+            considering their center's angle to the center of all clients.
             This parameter controls the amount of overlap needed before two
             routes are evaluated.
 
-        Raises
-        ------
-        RuntimeError
-            When this method is called before registering route operators.
-            Operators can be registered using :meth:`~add_route_operator`.
-
         Returns
         -------
         Solution
             The improved solution. This is not the same object as the
             solution that was passed in.
         """
         self._ls.shuffle(self._rng)
-        return self._ls.intensify(
-            solution, cost_evaluator, overlap_tolerance_degrees
-        )
+        return self._ls.intensify(solution, cost_evaluator, overlap_tolerance)
 
     def search(
         self, solution: Solution, cost_evaluator: CostEvaluator
     ) -> Solution:
         """
         This method uses the node operators on this local search object to
         improve the given solution.
@@ -180,20 +152,14 @@
         Parameters
         ----------
         solution
             The solution to improve.
         cost_evaluator
             Cost evaluator to use.
 
-        Raises
-        ------
-        RuntimeError
-            When this method is called before registering node operators.
-            Operators can be registered using :meth:`~add_node_operator`.
-
         Returns
         -------
         Solution
             The improved solution. This is not the same object as the
             solution that was passed in.
         """
         self._ls.shuffle(self._rng)
```

### Comparing `pyvrp-0.4.4/pyvrp/search/__init__.py` & `pyvrp-0.5.0/pyvrp/search/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .LocalSearch import LocalSearch
+from .SearchMethod import SearchMethod
 from ._search import (
     Exchange10,
     Exchange11,
     Exchange20,
     Exchange21,
     Exchange22,
     Exchange30,
```

### Comparing `pyvrp-0.4.4/pyvrp/search/_search.pyi` & `pyvrp-0.5.0/pyvrp/search/_search.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from typing import List
 
-from pyvrp._pyvrp import CostEvaluator, ProblemData, Solution, XorShift128
+from pyvrp._pyvrp import (
+    CostEvaluator,
+    ProblemData,
+    RandomNumberGenerator,
+    Solution,
+)
 
 class NodeOperator:
     def __init__(self, *args, **kwargs) -> None: ...
 
 class RouteOperator:
     def __init__(self, *args, **kwargs) -> None: ...
 
@@ -41,20 +46,25 @@
         data: ProblemData,
         neighbours: List[List[int]],
     ) -> None: ...
     def add_node_operator(self, op: NodeOperator) -> None: ...
     def add_route_operator(self, op: RouteOperator) -> None: ...
     def set_neighbours(self, neighbours: List[List[int]]) -> None: ...
     def get_neighbours(self) -> List[List[int]]: ...
-    def shuffle(self, rng: XorShift128) -> None: ...
+    def __call__(
+        self,
+        solution: Solution,
+        cost_evaluator: CostEvaluator,
+    ) -> Solution: ...
+    def shuffle(self, rng: RandomNumberGenerator) -> None: ...
     def intensify(
         self,
         solution: Solution,
         cost_evaluator: CostEvaluator,
-        overlap_tolerance_degrees: int = 0,
+        overlap_tolerance: float = 0.05,
     ) -> Solution: ...
     def search(
         self, solution: Solution, cost_evaluator: CostEvaluator
     ) -> Solution: ...
 
 class MoveTwoClientsReversed(NodeOperator):
     def __init__(self, data: ProblemData) -> None: ...
```

### Comparing `pyvrp-0.4.4/pyvrp/search/neighbourhood.py` & `pyvrp-0.5.0/pyvrp/search/neighbourhood.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import List
+from typing import TYPE_CHECKING, List
 
 import numpy as np
 
-from pyvrp import ProblemData
+if TYPE_CHECKING:
+    from pyvrp import ProblemData
 
 
 @dataclass
 class NeighbourhoodParams:
     """
     Configuration for calculating a granular neighbourhood.
 
@@ -76,25 +77,26 @@
         params.weight_wait_time,
         params.weight_time_warp,
     )
 
     if params.symmetric_proximity:
         proximity = np.minimum(proximity, proximity.T)
 
+    # TODO generalise this when we have multiple depots
     n = len(proximity)
     k = min(params.nb_granular, n - 2)  # excl. depot and self
 
     np.fill_diagonal(proximity, np.inf)  # cannot be in own neighbourhood
     proximity[0, :] = np.inf  # depot has no neighbours
     proximity[:, 0] = np.inf  # clients do not neighbour depot
 
     top_k = np.argsort(proximity, axis=1, kind="stable")[1:, :k]  # excl. depot
 
     if not params.symmetric_neighbours:
-        return [[]] + top_k.tolist()
+        return [[], *top_k.tolist()]
 
     # Construct a symmetric adjacency matrix and return the adjacent clients
     # as the neighbourhood structure.
     adj = np.zeros_like(proximity, dtype=bool)
     rows = np.expand_dims(np.arange(1, n), axis=1)
     adj[rows, top_k] = True
     adj = adj | adj.transpose()
```

### Comparing `pyvrp-0.4.4/pyvrp/search/tests/test_Exchange.py` & `pyvrp-0.5.0/pyvrp/search/tests/test_Exchange.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from numpy.testing import assert_, assert_equal
 from pytest import mark
 
 from pyvrp import (
     Client,
     CostEvaluator,
     ProblemData,
+    RandomNumberGenerator,
     Route,
     Solution,
     VehicleType,
-    XorShift128,
 )
 from pyvrp.search import (
     Exchange10,
     Exchange11,
     Exchange20,
     Exchange21,
     Exchange22,
@@ -42,15 +42,15 @@
     """
     Swap operators ((N, M)-exchange operators with M > 0) on a single route can
     only move within the same route, so they can never find a solution that has
     more than one route.
     """
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(operator(data))
 
     single_route = list(range(1, data.num_clients + 1))
     sol = Solution(data, [single_route])
@@ -74,15 +74,15 @@
 def test_relocate_uses_empty_routes(operator):
     """
     Unlike the swapping exchange operators, relocate should be able to relocate
     clients to empty routes if that is an improvement.
     """
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(operator(data))
 
     single_route = list(range(1, data.num_clients + 1))
     sol = Solution(data, [single_route])
@@ -111,15 +111,15 @@
     (N, M)-exchange works by exchanging N nodes starting at some node U with
     M nodes starting at some node V. But when there is no sequence of N or M
     nodes that does not contain the depot (because the routes are very short),
     then no exchange is possible.
     """
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(operator(data))
 
     sol = Solution(data, [[1, 2], [3], [4]])
     new_sol = ls.search(sol, cost_evaluator)
@@ -131,15 +131,15 @@
 def test_cannot_exchange_when_segments_overlap(operator):
     """
     (3, 2)- and (3, 3)-exchange cannot exchange anything on a length-four
     single route solution: there's always overlap between the segments.
     """
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(operator(data))
 
     sol = Solution(data, [[1, 2, 3, 4]])
     new_sol = ls.search(sol, cost_evaluator)
@@ -150,15 +150,15 @@
 def test_cannot_swap_adjacent_segments():
     """
     (2, 2)-exchange on a single route cannot swap adjacent segments, since
     that's already covered by (2, 0)-exchange.
     """
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(Exchange22(data))
 
     # An adjacent swap by (2, 2)-exchange could have created the single-route
     # solution [3, 4, 1, 2], which has a much lower cost. But that's not
@@ -172,15 +172,15 @@
 def test_swap_between_routes_OkSmall():
     """
     On the OkSmall example, (2, 1)-exchange should be able to swap parts of a
     two route solution, resulting in something better.
     """
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(Exchange21(data))
 
     sol = Solution(data, [[1, 2], [3, 4]])
     improved_sol = ls.search(sol, cost_evaluator)
@@ -195,15 +195,15 @@
 def test_relocate_after_depot_should_work():
     """
     This test exercises the bug identified in issue #142, involving a relocate
     action that should insert directly after the depot.
     """
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     # This is a non-empty neighbourhood (so LS does not complain), but the only
     # client moves allowed by it will not improve the initial solution created
     # below. So the only improvements (1, 0)-exchange can make must come from
     # moving clients behind the depot of a route.
     neighbours = [[] for _ in range(data.num_clients + 1)]
     neighbours[2].append(1)
@@ -218,15 +218,15 @@
     expected = Solution(data, [[1, 2], [3], [4]])
     assert_equal(ls.search(sol, cost_evaluator), expected)
 
 
 def test_relocate_only_happens_when_distance_and_duration_allow_it():
     """
     Tests that (1, 0)-exchange checks the duration matrix for time-window
-    feasibility before applying a move that improves the traveled distance.
+    feasibility before applying a move that improves the travelled distance.
     """
     clients = [
         Client(x=0, y=0, demand=0, service_duration=0, tw_early=0, tw_late=10),
         Client(x=1, y=0, demand=0, service_duration=0, tw_early=0, tw_late=5),
         Client(x=2, y=0, demand=0, service_duration=0, tw_early=0, tw_late=5),
     ]
 
@@ -253,15 +253,15 @@
     duration_optimal = Solution(data, [[2, 1]])
     distance_optimal = Solution(data, [[1, 2]])
 
     assert_(distance_optimal.distance() < duration_optimal.distance())
     assert_(duration_optimal.time_warp() < distance_optimal.time_warp())
 
     cost_evaluator = CostEvaluator(1, 1)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
     ls = LocalSearch(data, rng, compute_neighbours(data))
     ls.add_node_operator(Exchange10(data))
 
     assert_equal(ls.search(duration_optimal, cost_evaluator), duration_optimal)
     assert_equal(ls.search(distance_optimal, cost_evaluator), duration_optimal)
 
 
@@ -270,15 +270,15 @@
     This test asserts that a customer will be relocated to a non-empty route
     with a different capacity even if there is another empty route in between.
     """
     vehicle_types = [VehicleType(cap, 1) for cap in [12, 5, 1, 3]]
     data = make_heterogeneous(read("data/OkSmall.txt"), vehicle_types)
     # Use a huge cost for load penalties to make other aspects irrelevant
     cost_evaluator = CostEvaluator(100_000, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     # This is a non-empty neighbourhood (so LS does not complain), but the only
     # client moves allowed by it will not improve the initial solution created
     # below. So the only improvements (1, 0)-exchange can make must come from
     # moving clients behind the depot of a route.
     neighbours = [[] for _ in range(data.num_clients + 1)]
     neighbours[2].append(1)
```

### Comparing `pyvrp-0.4.4/pyvrp/search/tests/test_LocalSearch.py` & `pyvrp-0.5.0/pyvrp/search/tests/test_LocalSearch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 from numpy.testing import assert_, assert_equal, assert_raises
 from pytest import mark
 
-from pyvrp import CostEvaluator, Route, Solution, VehicleType, XorShift128
+from pyvrp import (
+    CostEvaluator,
+    RandomNumberGenerator,
+    Route,
+    Solution,
+    VehicleType,
+)
 from pyvrp.search import (
     Exchange10,
     Exchange11,
     LocalSearch,
     NeighbourhoodParams,
+    RelocateStar,
+    SwapStar,
     compute_neighbours,
 )
 from pyvrp.search._search import LocalSearch as cpp_LocalSearch
 from pyvrp.tests.helpers import make_heterogeneous, read
 
 
-def test_local_search_raises_when_there_are_no_operators():
+def test_local_search_returns_same_solution_when_there_are_no_operators():
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     ls = LocalSearch(data, rng, compute_neighbours(data))
     sol = Solution.make_random(data, rng)
 
-    with assert_raises(RuntimeError):
-        ls.search(sol, cost_evaluator)
+    # No operators have been added, so these calls should be no-ops.
+    assert_equal(ls.search(sol, cost_evaluator), sol)
+    assert_equal(ls.intensify(sol, cost_evaluator), sol)
 
-    with assert_raises(RuntimeError):
-        ls.intensify(sol, cost_evaluator)
 
-
-def test_local_search_raises_when_neighbourhood_structure_is_empty():
+def test_local_search_returns_same_solution_with_empty_neighbourhood():
     data = read("data/OkSmall.txt")
-    rng = XorShift128(seed=42)
-
-    # Is completely empty neighbourhood, so there's nothing to do for the
-    # local search in this case.
-    neighbours = [[] for _ in range(data.num_clients + 1)]
-
-    with assert_raises(RuntimeError):
-        LocalSearch(data, rng, neighbours)
+    cost_evaluator = CostEvaluator(20, 6)
+    rng = RandomNumberGenerator(seed=42)
 
-    ls = LocalSearch(data, rng, compute_neighbours(data))
+    ls = LocalSearch(data, rng, [[] for _ in range(data.num_clients + 1)])
+    ls.add_node_operator(Exchange10(data))
+    ls.add_node_operator(Exchange11(data))
 
-    with assert_raises(RuntimeError):
-        ls.set_neighbours(neighbours)
+    # The search is completed after one iteration due to the empty
+    # neighbourhood. This also prevents moves involving empty routes,
+    # which are not explicitly forbidden by the empty neighbourhood.
+    sol = Solution.make_random(data, rng)
+    assert_equal(ls.search(sol, cost_evaluator), sol)
 
 
 @mark.parametrize("size", [1, 2, 3, 4, 6, 7])  # num_clients + 1 == 5
 def test_local_search_raises_when_neighbourhood_dimensions_do_not_match(size):
     data = read("data/OkSmall.txt")
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     # Each of the given sizes is either smaller than or bigger than desired.
     neighbours = [[] for _ in range(size)]
 
     with assert_raises(RuntimeError):
         LocalSearch(data, rng, neighbours)
 
@@ -60,28 +65,30 @@
 
     with assert_raises(RuntimeError):
         ls.set_neighbours(neighbours)
 
 
 def test_local_search_raises_when_neighbourhood_contains_self_or_depot():
     data = read("data/OkSmall.txt")
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     neighbours = [[client] for client in range(data.num_clients + 1)]
 
     with assert_raises(RuntimeError):
         LocalSearch(data, rng, neighbours)
 
 
 @mark.parametrize(
-    "weight_wait_time,"
-    "weight_time_warp,"
-    "nb_granular,"
-    "symmetric_proximity,"
-    "symmetric_neighbours",
+    (
+        "weight_wait_time",
+        "weight_time_warp",
+        "nb_granular",
+        "symmetric_proximity",
+        "symmetric_neighbours",
+    ),
     [
         (20, 20, 10, True, False),
         (20, 20, 10, True, True),
         # From original c++ implementation
         # (18, 20, 34, False),
         (18, 20, 34, True, True),
     ],
@@ -90,15 +97,15 @@
     weight_wait_time: int,
     weight_time_warp: int,
     nb_granular: int,
     symmetric_proximity: bool,
     symmetric_neighbours: bool,
 ):
     data = read("data/RC208.txt", "solomon", round_func="trunc")
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     params = NeighbourhoodParams(nb_granular=1)
     prev_neighbours = compute_neighbours(data, params)
     ls = LocalSearch(data, rng, prev_neighbours)
 
     params = NeighbourhoodParams(
         weight_wait_time,
@@ -130,15 +137,15 @@
     """
     This test reproduces a bug where loadSolution in LocalSearch.cpp would
     reset the timewarp for a route to 0 if the route was not changed. This
     would cause improving moves with a smaller timewarp not to be considered
     because the current cost doesn't count the current time warp.
     """
     data = read("data/OkSmall.txt")
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     sol = Solution(data, [[1, 2, 3, 4]])
 
     # We make neighbours only contain 1 -> 2, so the only feasible move
     # is changing [1, 2, 3, 4] into [2, 1, 3, 4] or moving one of the nodes
     # into its own route. Since those solutions have larger distance but
     # smaller time warp, they are considered improving moves with a
@@ -163,15 +170,15 @@
 
 
 def test_prize_collecting():
     """
     Tests that local search works on a small prize-collecting instance.
     """
     data = read("data/p06-2-50.vrp", round_func="dimacs")
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
     cost_evaluator = CostEvaluator(1, 1)
 
     sol = Solution.make_random(data, rng)
     sol_cost = cost_evaluator.penalised_cost(sol)
 
     # Random solutions are complete...
     assert_equal(sol.num_clients(), data.num_clients)
@@ -186,15 +193,15 @@
     # ...but an optimised prize-collecting solution is likely not complete.
     assert_(improved.num_clients() < sol.num_clients())
     assert_(improved_cost < sol_cost)
 
 
 def test_cpp_shuffle_results_in_different_solution():
     data = read("data/RC208.txt", "solomon", round_func="trunc")
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     ls = cpp_LocalSearch(data, compute_neighbours(data))
     ls.add_node_operator(Exchange10(data))
     ls.add_node_operator(Exchange11(data))
 
     cost_evaluator = CostEvaluator(1, 1)
     sol = Solution.make_random(data, rng)
@@ -211,15 +218,15 @@
     improved3 = ls.search(sol, cost_evaluator)
     assert_(improved3 != improved1)
 
 
 def test_route_vehicle_types_are_preserved_for_locally_optimal_solutions():
     # This test tests that we will preserve vehicle types
     data = read("data/RC208.txt", "solomon", round_func="trunc")
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     neighbours = compute_neighbours(data)
     ls = cpp_LocalSearch(data, neighbours)
     ls.add_node_operator(Exchange10(data))
     ls.add_node_operator(Exchange11(data))
 
     cost_evaluator = CostEvaluator(1, 1)
@@ -241,7 +248,131 @@
     routes = [Route(data, r.visits(), 1) for r in improved.get_routes()]
     improved = Solution(data, routes)
 
     # Doing the search should not find any further improvements thus not change
     # the solution, especially not change the vehicle types
     further_improved = ls.search(improved, cost_evaluator)
     assert_equal(further_improved, improved)
+
+
+def test_bugfix_vehicle_type_offsets():
+    """
+    See https://github.com/PyVRP/PyVRP/pull/292 for details. This exercises a
+    fix to a bug that would crash local search due to an incorrect internal
+    mapping of vehicle types to route indices if the next vehicle type had
+    more vehicles than the previous.
+    """
+    data = read("data/OkSmall.txt")
+    data = make_heterogeneous(data, [VehicleType(10, 1), VehicleType(10, 2)])
+
+    ls = cpp_LocalSearch(data, compute_neighbours(data))
+    ls.add_node_operator(Exchange10(data))
+
+    cost_evaluator = CostEvaluator(1, 1)
+
+    current = Solution(data, [Route(data, [1, 3], 1), Route(data, [2, 4], 1)])
+    current_cost = cost_evaluator.penalised_cost(current)
+
+    improved = ls.search(current, cost_evaluator)
+    improved_cost = cost_evaluator.penalised_cost(improved)
+
+    assert_(improved_cost <= current_cost)
+
+
+def test_intensify_overlap_tolerance():
+    data = read("data/RC208.txt", "solomon", round_func="trunc")
+    rng = RandomNumberGenerator(seed=42)
+
+    neighbours = compute_neighbours(data)
+    ls = LocalSearch(data, rng, neighbours)
+    ls.add_route_operator(RelocateStar(data))
+
+    cost_eval = CostEvaluator(1, 1)
+    sol = Solution.make_random(data, rng)
+
+    # Overlap tolerance is zero, so no routes should have overlap and thus
+    # no intensification should take place.
+    unchanged = ls.intensify(sol, cost_eval, overlap_tolerance=0)
+    assert_equal(unchanged, sol)
+
+    # But with full overlap tolerance, all routes should be checked. That
+    # should lead to an improvement over the random solution.
+    better = ls.intensify(sol, cost_eval, overlap_tolerance=1)
+    assert_(better != sol)
+    assert_(cost_eval.penalised_cost(better) < cost_eval.penalised_cost(sol))
+
+
+@mark.parametrize("tol", [-1.0, -0.01, 1.01, 10.9, 1000])
+def test_intensify_overlap_tolerance_raises_outside_unit_interval(tol):
+    data = read("data/RC208.txt", "solomon", round_func="trunc")
+    rng = RandomNumberGenerator(seed=42)
+
+    neighbours = compute_neighbours(data)
+    ls = LocalSearch(data, rng, neighbours)
+    ls.add_route_operator(RelocateStar(data))
+
+    cost_eval = CostEvaluator(1, 1)
+    sol = Solution.make_random(data, rng)
+
+    with assert_raises(RuntimeError):  # each tolerance value is outside [0, 1]
+        ls.intensify(sol, cost_eval, overlap_tolerance=tol)
+
+
+def test_no_op_results_in_same_solution():
+    data = read("data/OkSmall.txt")
+    rng = RandomNumberGenerator(seed=42)
+
+    cost_eval = CostEvaluator(1, 1)
+    sol = Solution.make_random(data, rng)
+
+    # Empty local search does not actually search anything, so it should return
+    # the exact same solution as what was passed in.
+    ls = LocalSearch(data, rng, compute_neighbours(data))
+    assert_equal(ls(sol, cost_eval), sol)
+    assert_equal(ls.search(sol, cost_eval), sol)
+    assert_equal(ls.intensify(sol, cost_eval), sol)
+
+
+def test_intensify_can_improve_solution_further():
+    data = read("data/RC208.txt", "solomon", round_func="trunc")
+    rng = RandomNumberGenerator(seed=11)
+
+    ls = LocalSearch(data, rng, compute_neighbours(data))
+    ls.add_node_operator(Exchange11(data))
+    ls.add_route_operator(SwapStar(data))
+
+    cost_eval = CostEvaluator(1, 1)
+
+    # The following solution is locally optimal w.r.t. the node operators. This
+    # solution cannot be improved further by repeated calls to ``search()``.
+    search_opt = ls.search(Solution.make_random(data, rng), cost_eval)
+    search_cost = cost_eval.penalised_cost(search_opt)
+
+    # But it can be improved further using the intensifying route operators,
+    # as the following solution shows.
+    intensify_opt = ls.intensify(search_opt, cost_eval)
+    intensify_cost = cost_eval.penalised_cost(intensify_opt)
+
+    print(search_cost, intensify_cost)
+    assert_(intensify_cost < search_cost)
+
+    # Both solutions are locally optimal. ``search_opt`` w.r.t. to the node
+    # operators, and ``intensify_opt`` w.r.t. to the route operators. Repeated
+    # calls to ``search()`` and ``intensify`` do not result in further
+    # improvements for such locally optimal solutions.
+    for _ in range(10):
+        assert_equal(ls.search(search_opt, cost_eval), search_opt)
+        assert_equal(ls.intensify(intensify_opt, cost_eval), intensify_opt)
+
+
+def test_local_search_raises_for_incomplete_solutions():
+    data = read("data/OkSmallPrizes.txt")
+    rng = RandomNumberGenerator(seed=42)
+
+    ls = LocalSearch(data, rng, compute_neighbours(data))
+    ls.add_node_operator(Exchange10(data))
+
+    cost_eval = CostEvaluator(1, 1)
+    sol = Solution(data, [[2], [3, 4]])  # 1 is required but not visited
+
+    with assert_raises(RuntimeError):
+        ls.search(sol, cost_eval)
```

### Comparing `pyvrp-0.4.4/pyvrp/search/tests/test_MoveTwoClientsReversed.py` & `pyvrp-0.5.0/pyvrp/search/tests/test_MoveTwoClientsReversed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from numpy.testing import assert_, assert_equal
 from pytest import mark
 
-from pyvrp import CostEvaluator, Solution, XorShift128
+from pyvrp import CostEvaluator, RandomNumberGenerator, Solution
 from pyvrp.search import (
     LocalSearch,
     MoveTwoClientsReversed,
     NeighbourhoodParams,
     compute_neighbours,
 )
 from pyvrp.tests.helpers import read
@@ -14,15 +14,15 @@
 def test_single_route_OkSmall():
     """
     This test checks that MoveTwoClientsReversed properly solves the small
     instance where we know what is going on.
     """
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(MoveTwoClientsReversed(data))
 
     sol = Solution(data, [[1, 4, 2, 3]])
     improved_sol = ls.search(sol, cost_evaluator)
@@ -48,15 +48,15 @@
         assert_(improved_cost <= other_cost)
 
 
 @mark.parametrize("seed", [2643, 2742, 2941, 3457, 4299, 4497, 6178, 6434])
 def test_RC208_instance(seed: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=seed)
+    rng = RandomNumberGenerator(seed=seed)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(MoveTwoClientsReversed(data))
 
     single_route = list(range(1, data.num_clients + 1))
     sol = Solution(data, [single_route])
```

### Comparing `pyvrp-0.4.4/pyvrp/search/tests/test_RelocateStar.py` & `pyvrp-0.5.0/pyvrp/search/tests/test_RelocateStar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from numpy.testing import assert_, assert_equal
 from pytest import mark
 
-from pyvrp import CostEvaluator, Solution, XorShift128
+from pyvrp import CostEvaluator, RandomNumberGenerator, Solution
 from pyvrp.search import (
     Exchange10,
     LocalSearch,
     NeighbourhoodParams,
     RelocateStar,
     compute_neighbours,
 )
@@ -16,27 +16,27 @@
     """
     With sufficiently large granular neighbourhoods, (1, 0)-Exchange and
     RELOCATE* find the exact same solutions. Only when the granular
     neighbourhood is restricted do these solutions start to differ.
     """
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
 
     ls.add_node_operator(Exchange10(data))
     ls.add_route_operator(RelocateStar(data))
 
     for _ in range(10):  # repeat a few times to really make sure
         sol = Solution.make_random(data, rng)
         exchange_sol = ls.search(sol, cost_evaluator)
         relocate_sol = ls.intensify(
-            exchange_sol, cost_evaluator, overlap_tolerance_degrees=360
+            exchange_sol, cost_evaluator, overlap_tolerance=1
         )
 
         # RELOCATE* applies the best (1, 0)-exchange moves between routes. But
         # when the granular neighbourhood covers the entire client space, that
         # best move has already been evaluated and applied by regular (1,0)
         # exchange. Thus, at this point the solution cannot be improved
         # further by RELOCATE*.
@@ -47,26 +47,26 @@
 def test_exchange10_and_relocate_star_differ_small_neighbourhoods(size: int):
     """
     This test restricts the sizes of the granular neighbourhoods, so now
     (1, 0)-Exchange and RELOCATE* should start to differ.
     """
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=size)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
 
     ls.add_node_operator(Exchange10(data))
     ls.add_route_operator(RelocateStar(data))
 
     sol = Solution.make_random(data, rng)
     exchange_sol = ls.search(sol, cost_evaluator)
     relocate_sol = ls.intensify(
-        exchange_sol, cost_evaluator, overlap_tolerance_degrees=360
+        exchange_sol, cost_evaluator, overlap_tolerance=1
     )
 
     # The original solution was not that great, so after (1, 0)-Exchange it
     # should have improved. But that operator is restricted by the size of the
     # granular neighbourhood, which limits the number of operators. RELOCATE*
     # overcomes some of that, and as a result, should be able to improve the
     # solution further.
```

### Comparing `pyvrp-0.4.4/pyvrp/search/tests/test_SwapStar.py` & `pyvrp-0.5.0/pyvrp/search/tests/test_SwapStar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from numpy.testing import assert_, assert_equal
 from pytest import mark
 
-from pyvrp import CostEvaluator, Solution, XorShift128
+from pyvrp import CostEvaluator, RandomNumberGenerator, Solution
 from pyvrp.search import (
     Exchange11,
     LocalSearch,
     NeighbourhoodParams,
     SwapStar,
     compute_neighbours,
 )
@@ -17,30 +17,30 @@
     SWAP* can move two clients to any position in the routes, whereas regular
     swap ((1, 1)-exchange) must reinsert each client in the other's position.
     Thus, SWAP* should still be able to identify additional improving moves
     after (1, 1)-exchange gets stuck.
     """
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     # For a fair comparison we should not hamper the node operator with
     # granularity restrictions.
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
 
     ls.add_node_operator(Exchange11(data))
     ls.add_route_operator(SwapStar(data))
 
     for _ in range(10):  # repeat a few times to really make sure
         sol = Solution.make_random(data, rng)
 
         swap_sol = ls.search(sol, cost_evaluator)
         swap_star_sol = ls.intensify(
-            swap_sol, cost_evaluator, overlap_tolerance_degrees=360
+            swap_sol, cost_evaluator, overlap_tolerance=1
         )
 
         # The regular swap operator should have been able to improve the random
         # solution. After swap gets stuck, SWAP* should still be able to
         # further improve the solution.
         current_cost = cost_evaluator.penalised_cost(sol)
         swap_cost = cost_evaluator.penalised_cost(swap_sol)
@@ -49,27 +49,25 @@
         assert_(swap_star_cost < swap_cost)
 
 
 @mark.parametrize("seed", [2643, 2742, 2941, 3457, 4299, 4497, 6178, 6434])
 def test_swap_star_on_RC208_instance(seed: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=seed)
+    rng = RandomNumberGenerator(seed=seed)
 
     ls = LocalSearch(data, rng, compute_neighbours(data))
     ls.add_route_operator(SwapStar(data))
 
     # Make an initial solution that consists of two routes, by randomly
     # splitting the single-route solution.
     route = list(range(1, data.num_clients + 1))
     split = rng.randint(data.num_clients)
     sol = Solution(data, [route[:split], route[split:]])
-    improved_sol = ls.intensify(
-        sol, cost_evaluator, overlap_tolerance_degrees=360
-    )
+    improved_sol = ls.intensify(sol, cost_evaluator, overlap_tolerance=1)
 
     # The new solution should strictly improve on our original solution, but
     # cannot use more routes since SWAP* does not create routes.
     assert_equal(improved_sol.num_routes(), 2)
     current_cost = cost_evaluator.penalised_cost(sol)
     improved_cost = cost_evaluator.penalised_cost(improved_sol)
     assert_(improved_cost < current_cost)
```

### Comparing `pyvrp-0.4.4/pyvrp/search/tests/test_TwoOpt.py` & `pyvrp-0.5.0/pyvrp/search/tests/test_TwoOpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from typing import List
 
 import numpy as np
 from numpy.testing import assert_, assert_equal
 from pytest import mark
 
-from pyvrp import CostEvaluator, Route, Solution, VehicleType, XorShift128
+from pyvrp import (
+    CostEvaluator,
+    RandomNumberGenerator,
+    Route,
+    Solution,
+    VehicleType,
+)
 from pyvrp.search import (
     LocalSearch,
     NeighbourhoodParams,
     TwoOpt,
     compute_neighbours,
 )
 from pyvrp.tests.helpers import make_heterogeneous, read
 
 
 def test_OkSmall_instance():
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(TwoOpt(data))
 
     sol = Solution(data, [[1, 2, 3, 4]])
     improved_sol = ls.search(sol, cost_evaluator)
@@ -54,15 +60,15 @@
     # the vehicle capacities. Depending on the (heterogeneous) capacities,
     # the move may or may not be improving and should be applied or not
     # The starting solution has routes [1, 3] and [2, 4] with demands 8, 10
     # the 2-opt solution has routes [1, 4] and [2, 3] with demands 10, 8
 
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(10000, 6)  # Large capacity penalty
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     # Now making it heterogenous, the same move should result in capacity
     # penalties and thus not be applied
     data = make_heterogeneous(data, vehicle_types)
 
     neighbours: List[List[int]] = [[], [2], [], [], []]  # only 1 -> 2
     ls = LocalSearch(data, rng, neighbours)
@@ -84,15 +90,15 @@
     assert_equal(improved_sol2, expected_sol)
 
 
 @mark.parametrize("seed", [2643, 2742, 2941, 3457, 4299, 4497, 6178, 6434])
 def test_RC208_instance(seed: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=seed)
+    rng = RandomNumberGenerator(seed=seed)
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(TwoOpt(data))
 
     single_route = list(range(1, data.num_clients + 1))
     sol = Solution(data, [single_route])
```

### Comparing `pyvrp-0.4.4/pyvrp/search/tests/test_neighbourhood.py` & `pyvrp-0.5.0/pyvrp/search/tests/test_neighbourhood.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 from pytest import mark
 
 from pyvrp.search import NeighbourhoodParams, compute_neighbours
 from pyvrp.tests.helpers import read
 
 
 @mark.parametrize(
-    "weight_wait_time,"
-    "weight_time_warp,"
-    "nb_granular,"
-    "symmetric_proximity,"
-    "symmetric_neighbours",
+    (
+        "weight_wait_time",
+        "weight_time_warp",
+        "nb_granular",
+        "symmetric_proximity",
+        "symmetric_neighbours",
+    ),
     [
         # empty neighbourhood structure (nb_granular == 0)
         (20, 20, 0, True, False),
     ],
 )
 def test_neighbourhood_params_raises_for_invalid_arguments(
     weight_wait_time: int,
@@ -33,19 +35,21 @@
             nb_granular,
             symmetric_proximity,
             symmetric_neighbours,
         )
 
 
 @mark.parametrize(
-    "weight_wait_time,"
-    "weight_time_warp,"
-    "nb_granular,"
-    "symmetric_proximity,"
-    "symmetric_neighbours",
+    (
+        "weight_wait_time",
+        "weight_time_warp",
+        "nb_granular",
+        "symmetric_proximity",
+        "symmetric_neighbours",
+    ),
     [
         # non-empty neighbourhood structure (nb_granular > 0)
         (20, 20, 1, True, False),
         # no weights for wait time or time warp should be OK
         (0, 0, 1, True, False),
     ],
 )
@@ -62,21 +66,23 @@
         nb_granular,
         symmetric_proximity,
         symmetric_neighbours,
     )
 
 
 @mark.parametrize(
-    "weight_wait_time,"
-    "weight_time_warp,"
-    "nb_granular,"
-    "symmetric_proximity,"
-    "symmetric_neighbours,"
-    "idx_check,"
-    "expected_neighbours_check",
+    (
+        "weight_wait_time",
+        "weight_time_warp",
+        "nb_granular",
+        "symmetric_proximity",
+        "symmetric_neighbours",
+        "idx_check",
+        "expected_neighbours_check",
+    ),
     [
         # fmt: off
         (20, 20, 10, True, False, 2,
          {1, 3, 4, 5, 6, 7, 8, 45, 46, 100}),
         (20, 20, 10, True, True, 2,
          {1, 3, 4, 5, 6, 7, 8, 45, 46, 60, 70, 79, 100}),
         # From original c++ implementation
```

### Comparing `pyvrp-0.4.4/pyvrp/show_versions.py` & `pyvrp-0.5.0/pyvrp/show_versions.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/stop/MaxRuntime.py` & `pyvrp-0.5.0/pyvrp/stop/MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/stop/NoImprovement.py` & `pyvrp-0.5.0/pyvrp/stop/NoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/stop/StoppingCriterion.py` & `pyvrp-0.5.0/pyvrp/stop/StoppingCriterion.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,7 @@
             Cost of current best solution.
 
         Returns
         -------
         bool
             True if the algorithm should stop, False otherwise.
         """
-        ...
```

### Comparing `pyvrp-0.4.4/pyvrp/stop/TimedNoImprovement.py` & `pyvrp-0.5.0/pyvrp/stop/TimedNoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/stop/tests/test_MaxIterations.py` & `pyvrp-0.5.0/pyvrp/stop/tests/test_MaxIterations.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/stop/tests/test_MaxRuntime.py` & `pyvrp-0.5.0/pyvrp/stop/tests/test_MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/stop/tests/test_NoImprovement.py` & `pyvrp-0.5.0/pyvrp/stop/tests/test_NoImprovement.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     for _ in range(n):
         assert_(not stop(1))
 
     for _ in range(n):
         assert_(stop(1))
 
 
-@mark.parametrize("n, k", [(10, 2), (100, 20), (1000, 200)])
+@mark.parametrize(("n", "k"), [(10, 2), (100, 20), (1000, 200)])
 def test_n_max_iterations_with_single_improvement(n, k):
     """
     Test if setting max_iterations to n correctly stops with a sequence of
     solutions, when the k-th solution is improving and the other solutions
     are non-improving. The first n + k - 1 iterations should not stop. After
     that, the criterion should stop.
     """
```

### Comparing `pyvrp-0.4.4/pyvrp/stop/tests/test_TimedNoImprovement.py` & `pyvrp-0.5.0/pyvrp/stop/tests/test_TimedNoImprovement.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from pytest import mark
 
 from pyvrp.stop import TimedNoImprovement
 from pyvrp.tests.helpers import sleep
 
 
 @mark.parametrize(
-    "max_iterations, max_runtime",
+    ("max_iterations", "max_runtime"),
     [(-1, 0), (-42, 0), (-10_000, 0), (0, -1), (0, -42), (0, -10_000)],
 )
 def test_raise_negative_parameters(max_iterations, max_runtime):
     with assert_raises(ValueError):
         TimedNoImprovement(max_iterations, max_runtime)
 
 
 @mark.parametrize(
-    "max_iterations, max_runtime", [(0, 0.001), (1, 0.01), (10, 0.0)]
+    ("max_iterations", "max_runtime"), [(0, 0.001), (1, 0.01), (10, 0.0)]
 )
 def test_valid_parameters(max_iterations, max_runtime):
     """
     Does not raise for non-negative parameters.
     """
     TimedNoImprovement(max_iterations, max_runtime)
```

### Comparing `pyvrp-0.4.4/pyvrp/tests/data/E-n22-k4.txt` & `pyvrp-0.5.0/pyvrp/tests/data/E-n22-k4.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/data/EdgeWeightsNoExplicit.txt` & `pyvrp-0.5.0/pyvrp/tests/data/EdgeWeightsNoExplicit.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt` & `pyvrp-0.5.0/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/data/OkSmall.txt` & `pyvrp-0.5.0/pyvrp/tests/data/OkSmall.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/data/OkSmallGreedyRepair.txt` & `pyvrp-0.5.0/pyvrp/tests/data/OkSmallGreedyRepair.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/data/OkSmallPrizes.txt` & `pyvrp-0.5.0/pyvrp/tests/data/OkSmallPrizes.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/data/OkSmallReleaseTimes.txt` & `pyvrp-0.5.0/pyvrp/tests/data/OkSmallReleaseTimes.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/data/RC208.txt` & `pyvrp-0.5.0/pyvrp/tests/data/RC208.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/data/ReallyLargeDistance.txt` & `pyvrp-0.5.0/pyvrp/tests/data/ReallyLargeDistance.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/data/p06-2-50.vrp` & `pyvrp-0.5.0/pyvrp/tests/data/p06-2-50.vrp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/helpers.py` & `pyvrp-0.5.0/pyvrp/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_CostEvaluator.py` & `pyvrp-0.5.0/pyvrp/tests/test_CostEvaluator.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_DynamicBitset.py` & `pyvrp-0.5.0/pyvrp/tests/test_DynamicBitset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from numpy.testing import assert_, assert_equal
 from pytest import mark
 
 from pyvrp._pyvrp import DynamicBitset
 
 
 @mark.parametrize(
-    "num_bits, expected_size",
+    ("num_bits", "expected_size"),
     [(0, 0), (1, 64), (64, 64), (65, 128), (128, 128)],
 )
 def test_size(num_bits, expected_size):
     """
     The bitset size is increased in increments of 64 bits.
     """
     bitset = DynamicBitset(num_bits)
```

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_Matrix.py` & `pyvrp-0.5.0/pyvrp/tests/test_Matrix.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_Model.py` & `pyvrp-0.5.0/pyvrp/tests/test_Model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from numpy.testing import assert_, assert_equal, assert_raises, assert_warns
 from pytest import mark
 
 from pyvrp import Model
 from pyvrp.constants import MAX_USER_VALUE, MAX_VALUE
-from pyvrp.exceptions import ScalingWarning
+from pyvrp.exceptions import EmptySolutionWarning, ScalingWarning
 from pyvrp.stop import MaxIterations
 from pyvrp.tests.helpers import read
 
 
 def test_model_data():
     model = Model()
 
@@ -42,15 +42,15 @@
         model.add_edge(client, depot, distance=-1, duration=0)
 
     with assert_raises(ValueError):  # negative duration should also not be OK
         model.add_edge(client, depot, distance=0, duration=-1)
 
 
 @mark.parametrize(
-    "number, capacity",
+    ("number", "capacity"),
     [
         (0, 1),  # zero vehicles is not OK (but zero capacity is)
         (-1, 1),  # negative vehicles is not OK
         (1, -1),  # negative capacity is not OK
     ],
 )
 def test_add_vehicle_type_raises_negative_number_or_capacity(number, capacity):
@@ -253,7 +253,33 @@
         model.data()
         assert_equal(len(recwarn), 0)
 
     # But a value exceeding the maximum user value is not OK. This should warn.
     model.add_edge(depot, client, distance=MAX_USER_VALUE + 1)
     with assert_warns(ScalingWarning):
         model.data()
+
+
+def test_model_solves_instance_with_zero_or_one_clients():
+    """
+    This test exercises the bug identified in issue #272, where the model
+    could not solve an instance with zero clients or just one client.
+    """
+    m = Model()
+    m.add_vehicle_type(capacity=15, num_available=1)
+    depot = m.add_depot(x=0, y=0)
+
+    # Solve an instance with no clients.
+    with assert_warns(EmptySolutionWarning):
+        res = m.solve(stop=MaxIterations(1))
+
+    solution = [r.visits() for r in res.best.get_routes()]
+    assert_equal(solution, [])
+
+    # Solve an instance with one client.
+    clients = [m.add_client(x=0, y=0, demand=0)]
+    m.add_edge(depot, clients[0], distance=0)
+    m.add_edge(clients[0], depot, distance=0)
+
+    res = m.solve(stop=MaxIterations(1))
+    solution = [r.visits() for r in res.best.get_routes()]
+    assert_equal(solution, [[1]])
```

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_PenaltyManager.py` & `pyvrp-0.5.0/pyvrp/tests/test_PenaltyManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from numpy.testing import assert_equal, assert_raises
 from pytest import mark
 
 from pyvrp import PenaltyManager, PenaltyParams
 
 
 @mark.parametrize(
-    "init_load_penalty,"
-    "init_tw_penalty,"
-    "repair_booster,"
-    "num_iters_between_penalty_updates,"
-    "penalty_increase,"
-    "penalty_decrease,"
-    "target_feasible",
+    (
+        "init_load_penalty",
+        "init_tw_penalty",
+        "repair_booster",
+        "num_iters_between_penalty_updates",
+        "penalty_increase",
+        "penalty_decrease",
+        "target_feasible",
+    ),
     [
         (1, 1, 1, 0, -1.0, 0.5, 0.5),  # -1 penalty increase
         (1, 1, 1, 0, 0.5, 0.5, 0.5),  # 0.5 penalty increase
         (1, 1, 1, 0, 1.5, -1, 0.5),  # -1 penalty decrease
         (1, 1, 1, 0, 1.5, 2, 0.5),  # 2 penalty decrease
         (1, 1, 1, 0, 1, 1, -1),  # -1 target feasible
         (1, 1, 1, 0, 1, 1, 2),  # 2 target feasible
```

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_Population.py` & `pyvrp-0.5.0/pyvrp/tests/test_Population.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 )
 from pytest import mark
 
 from pyvrp import (
     CostEvaluator,
     Population,
     PopulationParams,
+    RandomNumberGenerator,
     Solution,
-    XorShift128,
 )
 from pyvrp.diversity import broken_pairs_distance as bpd
 from pyvrp.exceptions import EmptySolutionWarning
 from pyvrp.tests.helpers import make_random_solutions, read
 
 
 @mark.parametrize(
-    "min_pop_size,"
-    "generation_size,"
-    "nb_elite,"
-    "nb_close,"
-    "lb_diversity,"
-    "ub_diversity",
+    (
+        "min_pop_size",
+        "generation_size",
+        "nb_elite",
+        "nb_close",
+        "lb_diversity",
+        "ub_diversity",
+    ),
     [
         (1, 1, 1, 1, -1, 1.0),  # -1 lb_diversity
         (1, 1, 1, 1, 2, 1.0),  # 2 lb_diversity
         (1, 1, 1, 1, 0, -1.0),  # -1 ub_diversity
         (1, 1, 1, 1, 0, 2.0),  # 2 ub_diversity
         (1, 1, 1, 1, 1, 0.5),  # ub_diversity < lb_diversity
         (1, 1, 1, 1, 0.5, 0.5),  # ub_diversity == lb_diversity
@@ -55,20 +57,22 @@
             nb_close,
             lb_diversity,
             ub_diversity,
         )
 
 
 @mark.parametrize(
-    "min_pop_size,"
-    "generation_size,"
-    "nb_elite,"
-    "nb_close,"
-    "lb_diversity,"
-    "ub_diversity",
+    (
+        "min_pop_size",
+        "generation_size",
+        "nb_elite",
+        "nb_close",
+        "lb_diversity",
+        "ub_diversity",
+    ),
     [
         (1, 1, 1, 1, 0.0, 0.5),  # >0 min_pop_size
         (1, 0, 1, 1, 0.0, 0.5),  # 0 generation_size
         (1, 1, 0, 1, 0.0, 0.5),  # 0 nb_elite
         (1, 1, 1, 0, 0.0, 0.5),  # 0 nb_close
         (1, 1, 1, 1, 0.0, 0.5),  # 0 lb_diversity
         (1, 1, 1, 1, 0.0, 1.0),  # 1 ub_diversity
@@ -102,15 +106,15 @@
     assert_allclose(params.ub_diversity, ub_diversity)
     assert_equal(params.max_pop_size, min_pop_size + generation_size)
 
 
 def test_add_triggers_purge():
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     params = PopulationParams()
     pop = Population(bpd, params=params)
 
     for sol in make_random_solutions(params.min_pop_size, data, rng):
         pop.add(sol, cost_evaluator)
 
@@ -146,15 +150,15 @@
     assert_equal(pop.num_feasible(), params.min_pop_size)
     assert_equal(len(pop), num_infeas + params.min_pop_size)
 
 
 def test_select_returns_same_parents_if_no_other_option():
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=2_147_483_647)
+    rng = RandomNumberGenerator(seed=2_147_483_647)
 
     params = PopulationParams(min_pop_size=0)
     pop = Population(bpd, params=params)
 
     assert_equal(len(pop), 0)
 
     pop.add(Solution(data, [[3, 2], [1, 4]]), cost_evaluator)
@@ -186,15 +190,15 @@
 
 # // TODO test more select() - diversity, feas/infeas pairs
 
 
 def test_population_is_empty_with_zero_min_pop_size_and_generation_size():
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=12)
+    rng = RandomNumberGenerator(seed=12)
 
     params = PopulationParams(min_pop_size=0, generation_size=0)
     pop = Population(bpd, params=params)
 
     assert_equal(len(pop), 0)
 
     for _ in range(10):
@@ -206,15 +210,15 @@
 
 
 @mark.parametrize("nb_elite", [5, 25])
 def test_elite_solutions_are_not_purged(nb_elite: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
     params = PopulationParams(nb_elite=nb_elite)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     pop = Population(bpd, params=params)
 
     # Keep adding solutions until the infeasible subpopulation is of maximum
     # size.
     while pop.num_infeasible() != params.max_pop_size:
         pop.add(Solution.make_random(data, rng), cost_evaluator)
@@ -241,29 +245,29 @@
         assert_(id(elite_sol) in new_sols)
 
 
 @mark.parametrize("k", [2, 3])
 def test_tournament_ranks_by_fitness(k: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
     pop = Population(bpd)
 
     for sol in make_random_solutions(50, data, rng):
         if not sol.is_feasible():
             pop.add(sol, cost_evaluator)
 
     assert_equal(pop.num_feasible(), 0)
 
     # Since this test requires the fitness values of the solutions, we have
     # to access the underlying infeasible subpopulation directly.
-    infeas_pop = pop._infeas
+    infeas_pop = pop._infeas  # noqa: SLF001
     infeas_pop.update_fitness(cost_evaluator)
 
-    items = [item for item in pop._infeas]
+    items = [item for item in infeas_pop]
     by_fitness = sorted(items, key=lambda item: item.fitness)
     sol2idx = {item.solution: idx for idx, item in enumerate(by_fitness)}
     infeas_count = np.zeros(len(infeas_pop))
 
     for _ in range(10_000):
         sol = pop.get_tournament(rng, cost_evaluator, k=k)
         infeas_count[sol2idx[sol]] += 1
@@ -286,29 +290,29 @@
     assert_allclose(actual_freq, expected_freq, atol=0.01)  # 1% tolerance
 
 
 @mark.parametrize("k", [-100, -1, 0])  # k must be strictly positive
 def test_tournament_raises_for_invalid_k(k: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
     pop = Population(bpd)
 
     for sol in make_random_solutions(5, data, rng):
         pop.add(sol, cost_evaluator)
 
     with assert_raises(ValueError):
         pop.get_tournament(rng, cost_evaluator, k=k)
 
 
 def test_purge_removes_duplicates():
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
     params = PopulationParams(min_pop_size=20, generation_size=5)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     pop = Population(bpd, params=params)
 
     for sol in make_random_solutions(params.min_pop_size, data, rng):
         pop.add(sol, cost_evaluator)
 
     assert_equal(len(pop), params.min_pop_size)
@@ -339,15 +343,15 @@
     duplicates = sum(other == sol for other in pop)
     assert_equal(duplicates, 1)
 
 
 def test_clear():
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
     pop = Population(bpd)
 
     for sol in make_random_solutions(10, data, rng):
         pop.add(sol, cost_evaluator)
 
     assert_equal(len(pop), 10)
```

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_ProblemData.py` & `pyvrp-0.5.0/pyvrp/tests/test_ProblemData.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import numpy as np
 from numpy.random import default_rng
-from numpy.testing import assert_, assert_allclose, assert_raises
+from numpy.testing import assert_allclose, assert_raises
 from pytest import mark
 
 from pyvrp import Client, ProblemData, VehicleType
 from pyvrp.tests.helpers import read
 
 
 @mark.parametrize(
-    "x,y,demand,service_duration,tw_early,tw_late,release_time,prize",
+    (
+        "x",
+        "y",
+        "demand",
+        "service_duration",
+        "tw_early",
+        "tw_late",
+        "release_time",
+        "prize",
+    ),
     [
         (1, 1, 1, 1, 0, 1, 0, 0),  # normal
         (1, 1, 1, 0, 0, 1, 0, 0),  # zero duration
         (1, 1, 0, 1, 0, 1, 0, 0),  # zero demand
         (1, 1, 1, 1, 0, 0, 0, 0),  # zero length time interval
         (-1, -1, 1, 1, 0, 1, 0, 0),  # negative coordinates
         (1, 1, 1, 1, 0, 1, 1, 0),  # positive release time
@@ -39,15 +48,24 @@
     assert_allclose(client.tw_early, tw_early)
     assert_allclose(client.tw_late, tw_late)
     assert_allclose(client.release_time, release_time)
     assert_allclose(client.prize, prize)
 
 
 @mark.parametrize(
-    "x,y,demand,service,tw_early,tw_late,release_time,prize",
+    (
+        "x",
+        "y",
+        "demand",
+        "service",
+        "tw_early",
+        "tw_late",
+        "release_time",
+        "prize",
+    ),
     [
         (1, 1, 1, 1, 1, 0, 0, 0),  # late < early
         (1, 1, 1, -1, 0, 1, 0, 0),  # negative service duration
         (1, 1, -1, 1, 0, 1, 0, 0),  # negative demand
         (1, 1, 1, 1, 0, 1, 0, -1),  # negative prize
     ],
 )
@@ -61,29 +79,85 @@
     release_time: int,
     prize: int,
 ):
     with assert_raises(ValueError):
         Client(x, y, demand, service, tw_early, tw_late, release_time, prize)
 
 
-def test_depot_is_first_client():
+@mark.parametrize(
+    "x,y,demand,service,tw_early,tw_late,release_time,prize",
+    [
+        (0, 0, 1, 0, 0, 0, 0, 0),  # demand != 0
+        (0, 0, 0, 1, 0, 0, 0, 0),  # service duration != 0
+        (0, 0, 0, 0, 0, 0, 1, 0),  # release time != 0
+    ],
+)
+def test_raises_for_invalid_depot_data(
+    x: int,
+    y: int,
+    demand: int,
+    service: int,
+    tw_early: int,
+    tw_late: int,
+    release_time: int,
+    prize: int,
+):
+    depot = Client(
+        x, y, demand, service, tw_early, tw_late, release_time, prize
+    )
+
+    with assert_raises(ValueError):
+        ProblemData([depot], [VehicleType(1, 2)], [[0]], [[0]])
+
+
+def test_problem_data_raises_when_no_clients_provided():
     """
-    The ``depot()`` helper should return the first client, that is,
-    ``client(0)``.
+    Tests that the ``ProblemData`` constructor raises a ``ValueError`` when
+    no clients are provided.
     """
-    mat = [[0, 1], [1, 0]]
-
-    data = ProblemData(
-        clients=[Client(x=0, y=0), Client(x=0, y=1)],
+    with assert_raises(ValueError):
+        ProblemData(
+            clients=[],
+            vehicle_types=[VehicleType(1, 2)],
+            distance_matrix=[],
+            duration_matrix=[],
+        )
+
+    # One client (the depot) should not raise.
+    ProblemData(
+        clients=[Client(x=0, y=0)],
         vehicle_types=[VehicleType(1, 2)],
-        distance_matrix=mat,
-        duration_matrix=mat,
+        distance_matrix=[[0]],
+        duration_matrix=[[0]],
     )
 
-    assert_(data.depot() is data.client(0))
+
+@mark.parametrize(
+    "matrix",
+    [
+        [[0, 0]],  # num rows < num clients
+        [[], []],  # num cols < num clients
+        [[0, 0], [0, 0], [0, 0]],  # num rows > num clients
+        [[0, 0, 0], [0, 0, 0]],  # num cols > num clients
+    ],
+)
+def test_problem_data_raises_when_incorrect_matrix_dimensions(matrix):
+    """
+    Tests that the ``ProblemData`` constructor raises a ``ValueError`` when
+    the distance or duration matrix does not match the number of clients in
+    dimension size.
+    """
+    clients = [Client(x=0, y=0), Client(x=0, y=0)]
+    vehicle_types = [VehicleType(1, 2)]
+
+    with assert_raises(ValueError):
+        ProblemData(clients, vehicle_types, matrix, [[0, 0], [0, 0]])
+
+    with assert_raises(ValueError):
+        ProblemData(clients, vehicle_types, [[0, 0], [0, 0]], matrix)
 
 
 def test_centroid():
     data = read("data/OkSmall.txt")
 
     centroid = data.centroid()
     x = [data.client(idx).x for idx in range(1, data.num_clients + 1)]
```

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_Solution.py` & `pyvrp-0.5.0/pyvrp/tests/test_Solution.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import numpy as np
 from numpy.testing import assert_, assert_allclose, assert_equal, assert_raises
 from pytest import mark
 
 from pyvrp import (
     Client,
     ProblemData,
+    RandomNumberGenerator,
     Route,
     Solution,
     VehicleType,
-    XorShift128,
 )
 from pyvrp.tests.helpers import make_heterogeneous, read
 
 
 def test_route_constructor_raises_for_empty_routes():
     data = read("data/OkSmall.txt")
 
@@ -43,14 +43,15 @@
     assert_equal(routes[1].visits(), [1, 2])
     assert_equal(routes[1].vehicle_type(), 1)
     assert_equal(routes[1], Route(data, [1, 2], 1))
 
 
 def test_route_eq():
     data = read("data/OkSmall.txt")
+    data = make_heterogeneous(data, [VehicleType(10, 1), VehicleType(20, 2)])
 
     route1 = Route(data, [1, 2], 0)
     assert_(route1 == route1)  # should equal self
 
     route2 = Route(data, [1, 2], 0)
     assert_equal(route1, route2)  # same route/vehicle type; different object
 
@@ -66,15 +67,15 @@
 
 
 def test_random_constructor_cycles_over_routes():
     # This instance has four clients and three vehicles. Since 1 client per
     # vehicle would not work (insufficient vehicles), each route is given two
     # clients (and the last route should be empty).
     data = read("data/OkSmall.txt")
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
 
     sol = Solution.make_random(data, rng)
     routes = sol.get_routes()
 
     assert_equal(sol.num_routes(), 2)
     assert_equal(len(routes), 2)
 
@@ -121,22 +122,40 @@
         sol = Solution(data, [Route(data, [1, 2], 1), Route(data, [4, 3], 1)])
 
     # Three routes should raise since they are considered to be type 0.
     with assert_raises(RuntimeError):
         Solution(data, [[1, 2], [4], [3]])
 
 
-def test_route_constructor_raises_for_invalid_routes():
+def test_route_constructor_raises_when_clients_are_visited_more_than_once():
     data = read("data/OkSmall.txt")
     with assert_raises(RuntimeError):
         Solution(data, [[1, 2], [1, 3, 4]])  # client 1 is visited twice
 
-    data = read("data/OkSmallPrizes.txt")
     with assert_raises(RuntimeError):
-        Solution(data, [[2], [3, 4]])  # 1 is required but not visited
+        Solution(data, [[1, 2], [1, 3, 4], [1]])  # client 1 is visited thrice
+
+
+def test_route_constructor_allows_incomplete_solutions():
+    data = read("data/OkSmallPrizes.txt")
+
+    # Client 1 is required but not visited.
+    sol = Solution(data, [[2], [3, 4]])
+    assert_(not sol.is_complete())
+    assert_(not sol.is_feasible())
+
+    # All required clients are visited, but the solution is not feasible.
+    sol = Solution(data, [[1], [2, 3, 4]])
+    assert_(not sol.is_feasible())
+    assert_(sol.is_complete())
+
+    # All required clients are visited and the solution is feasible.
+    sol = Solution(data, [[1]])
+    assert_(sol.is_feasible())
+    assert_(sol.is_complete())
 
 
 def test_get_neighbours():
     data = read("data/OkSmall.txt")
 
     sol = Solution(data, [[3, 4], [1, 2]])
     neighbours = sol.get_neighbours()
@@ -182,15 +201,15 @@
     # Client 1 is released at 20'000, but client 2 time window ends at 19'500,
     # so this solution must be infeasible due to time-warping. We arrive at
     # client 1 at time 20'000 + 1'544 = 21'544 before the TW closes (22'500).
     # We arrive at client 2 at 21'544 + 360 + 1'992 = 23'896, so we incur a
     # time warp of 23'896 - 19'500 = 4'396.
     sol = Solution(data, [[1, 2], [3], [4]])
     assert_(not sol.is_feasible())
-    assert_equal(sol.time_warp(), 4396)
+    assert_allclose(sol.time_warp(), 4396)
 
     # Visiting clients 2 and 3 together is feasible: both clients are released
     # at time 5'000. We arrive at client 2 at 5'000 + 1'944 and wait till the
     # TW opens (12'000). We arrive at client 3 at 12'000 + 360 + 621 = 12'981,
     # which is before the TW closes (15'300).
     sol = Solution(data, [[1], [2, 3], [4]])
     assert_(sol.is_feasible())
@@ -225,34 +244,34 @@
 
     sol = Solution(data, [[4, 3, 1, 2]])
     assert_(sol.has_excess_load())
     assert_(not sol.has_time_warp())
 
     # All clients are visited on the same route/by the same vehicle. The total
     # demand is 18, but the vehicle capacity is only 10.
-    assert_equal(sol.excess_load(), 18 - data.vehicle_type(0).capacity)
+    assert_allclose(sol.excess_load(), 18 - data.vehicle_type(0).capacity)
 
 
 def test_heterogeneous_capacity_excess_load_calculation():
     data = read("data/OkSmall.txt")
     data = make_heterogeneous(
         data, vehicle_types=[VehicleType(10, 2), VehicleType(20, 1)]
     )
 
     # This instance has capacities 10 and 20 for vehicle type 0 and 1. The
     # total demand is 18 so if all demand is put in vehicle type 0 the
     # excess_load is 18 - 10 = 8.
     sol = Solution(data, [Route(data, [1, 2, 3, 4], 0)])
     assert_(sol.has_excess_load())
-    assert_equal(sol.excess_load(), 8)
+    assert_allclose(sol.excess_load(), 8)
 
     # With vehicle type 1, the capacity 20 is larger than 18.
     sol = Solution(data, [Route(data, [1, 2, 3, 4], 1)])
     assert_(not sol.has_excess_load())
-    assert_equal(sol.excess_load(), 0)
+    assert_allclose(sol.excess_load(), 0)
 
 
 def test_route_access_methods():
     data = read("data/OkSmall.txt")
     sol = Solution(data, [[1, 3], [2, 4]])
     routes = sol.get_routes()
 
@@ -281,49 +300,137 @@
         data.client(idx).service_duration
         for idx in range(data.num_clients + 1)
     ]
     assert_allclose(routes[0].service_duration(), services[1] + services[3])
     assert_allclose(routes[1].service_duration(), services[2] + services[4])
 
 
-def test_route_time_warp_and_wait_duration():
+def test_route_time_warp_calculations():
     data = read("data/OkSmall.txt")
     sol = Solution(data, [[1, 3], [2, 4]])
     routes = sol.get_routes()
 
-    # There's only time warp on the first route: duration(0, 1) = 1'544, so we
+    # There is time warp on the first route: duration(0, 1) = 1'544, so we
     # arrive at 1 before its opening window of 15'600. Service (360) thus
     # starts at 15'600, and completes at 15'600 + 360. Then we drive for
     # duration(1, 3) = 1'427, where we arrive after 15'300 (its closing time
     # window). This is where we incur time warp: we need to 'warp' to 15'300.
     assert_(sol.has_time_warp())
     assert_(routes[0].has_time_warp())
-    assert_(not routes[1].has_time_warp())
     assert_allclose(routes[0].time_warp(), 15_600 + 360 + 1_427 - 15_300)
+
+    # The second route has no time warp, so the overall solution time warp is
+    # all incurred on the first route.
+    assert_(not routes[1].has_time_warp())
     assert_allclose(routes[1].time_warp(), 0)
     assert_allclose(sol.time_warp(), routes[0].time_warp())
 
-    # On the first route, we have to wait at the first client, where we arrive
-    # at 1'544, but cannot start service until 15'600. On the second route, we
-    # also have to wait at the first client, where we arrive at 1'944, but
-    # cannot start service until 12'000.
-    assert_equal(routes[0].wait_duration(), 15_600 - 1_544)
-    assert_equal(routes[1].wait_duration(), 12_000 - 1_944)
+
+def test_route_wait_time_calculations():
+    data = read("data/OkSmallWaitTime.txt")
+    sol = Solution(data, [[1, 3], [2, 4]])
+    routes = sol.get_routes()
+
+    # In the second route, the time window of client 2 closes at 15'000. After
+    # service and travel, we then arrive at client 4 before its time window is
+    # open, so we have to wait. In particular, we have to wait:
+    #   twEarly(4) - duration(2, 4) - serv(2) - twLate(2)
+    #     = 18'000 - 1'090 - 360 - 15'000
+    #     = 1'550.
+    assert_allclose(routes[1].wait_duration(), 1_550)
+
+    # Since there is waiting time, there is no slack in the schedule. We should
+    # thus start as late as possible, at:
+    #   twLate(2) - duration(0, 2)
+    #     = 15'000 - 1'944
+    #     = 13'056.
+    assert_allclose(routes[1].slack(), 0)
+    assert_allclose(routes[1].start_time(), 13_056)
+
+    # So far we have tested a route that had wait duration, but not time warp.
+    # We now test a solution with a route that has both.
+    sol = Solution(data, [[1, 2, 4], [3]])
+    route, *_ = sol.get_routes()
+
+    # This route has the same wait time as explained above. The time warp is
+    # incurred earlier in the route, between 1 -> 2:
+    #   twEarly(1) + serv(1) + duration(1, 2) - twLate(2)
+    #     = 15'600 + 360 + 1'992 - 15'000
+    #     = 2'952.
+    assert_allclose(route.time_warp(), 2_952)
+    assert_allclose(route.wait_duration(), 1_550)
+    assert_allclose(route.slack(), 0)
+
+    # Finally, the overall route duration should be equal to the sum of the
+    # travel, service, and waiting durations.
+    assert_allclose(
+        route.duration(),
+        route.travel_duration()
+        + route.service_duration()
+        + route.wait_duration(),
+    )
+
+
+def test_route_start_and_end_time_calculations():
+    data = read("data/OkSmall.txt")
+    sol = Solution(data, [[1, 3], [2, 4]])
+    routes = sol.get_routes()
+
+    # The first route has timewarp, so there is no slack in the schedule. We
+    # should thus depart as soon as possible to arrive at the first client the
+    # moment its time window opens.
+    start_time = data.client(1).tw_early - data.duration(0, 1)
+    end_time = start_time + routes[0].duration() - routes[0].time_warp()
+
+    assert_(routes[0].has_time_warp())
+    assert_allclose(routes[0].slack(), 0)
+    assert_allclose(routes[0].start_time(), start_time)
+    assert_allclose(routes[0].end_time(), end_time)
+
+    # The second route has no time warp. The latest it can start is calculated
+    # backwards from the closing of client 4's time window:
+    #   twLate(4) - duration(2, 4) - serv(2) - duration(0, 2)
+    #     = 19'500 - 1'090 - 360 - 1'944
+    #     = 16'106.
+    #
+    # Because client 4 has a large time window, the earliest this route can
+    # start is determined completely by client 2: we should not arrive before
+    # its time window, because that would incur needless waiting. We should
+    # thus not depart before:
+    #   twEarly(2) - duration(0, 2)
+    #     = 12'000 - 1'944
+    #     = 10'056.
+    assert_(not routes[1].has_time_warp())
+    assert_allclose(routes[1].wait_duration(), 0)
+    assert_allclose(routes[1].start_time(), 10_056)
+    assert_allclose(routes[1].slack(), 16_106 - 10_056)
+
+    # The overall route duration is given by:
+    #   duration(0, 2) + serv(2) + duration(2, 4) + serv(4) + duration(4, 0)
+    #     = 1'944 + 360 + 1'090 + 360 + 1'475
+    #     = 5'229.
+    assert_allclose(routes[1].duration(), 1_944 + 360 + 1_090 + 360 + 1_475)
+    assert_allclose(routes[1].end_time(), 10_056 + 5_229)
 
 
 def test_route_release_time():
     data = read("data/OkSmallReleaseTimes.txt")
     sol = Solution(data, [[1, 3], [2, 4]])
     routes = sol.get_routes()
 
-    # The client release times are 20'000, 5'000, 5'000 and 1'000.
-    # So the first route has a release time of max(20'000, 5'000) = 20'000,
-    # and the second route has a release time of max(5'000, 1'000) = 5'000.
-    assert_allclose(routes[0].release_time(), 20000)
-    assert_allclose(routes[1].release_time(), 5000)
+    # The client release times are 20'000, 5'000, 5'000 and 1'000. So the first
+    # route has a release time of max(20'000, 5'000) = 20'000, and the second
+    # has a release time of max(5'000, 1'000) = 5'000.
+    assert_allclose(routes[0].release_time(), 20_000)
+    assert_allclose(routes[1].release_time(), 5_000)
+
+    # Second route is feasible, so should have start time not smaller than
+    # release time.
+    assert_(not routes[1].has_time_warp())
+    assert_(routes[1].start_time() > routes[1].release_time())
 
 
 @mark.parametrize(
     "dist_mat",
     [
         np.full((3, 3), fill_value=100, dtype=int),
         np.full((3, 3), fill_value=1, dtype=int),
@@ -362,20 +469,42 @@
 
     # But visiting the second client after the first is feasible.
     feasible = Solution(data, [[1, 2]])
     assert_(not feasible.has_time_warp())
     assert_(not feasible.has_excess_load())
     assert_(feasible.is_feasible())
 
-    assert_equal(
+    assert_allclose(
         feasible.distance(),
         dist_mat[0, 1] + dist_mat[1, 2] + dist_mat[2, 0],
     )
 
 
+def test_time_warp_return_to_depot():
+    """
+    This tests wether the calculated total duration and time warp includes the
+    travel back to the depot.
+    """
+    data = ProblemData(
+        clients=[Client(x=0, y=0, tw_late=1), Client(x=1, y=0)],
+        vehicle_types=[VehicleType(0, 1)],
+        distance_matrix=[[0, 0], [0, 0]],
+        duration_matrix=[[0, 1], [1, 0]],
+    )
+
+    sol = Solution(data, [[1]])
+    route, *_ = sol.get_routes()
+
+    # Travel from depot to client and back gives duration 1 + 1 = 2. This is 1
+    # more than the depot time window 1, giving a time warp of 1.
+    assert_allclose(route.duration(), 2)
+    assert_allclose(data.client(0).tw_late, 1)
+    assert_allclose(sol.time_warp(), 1)
+
+
 # TODO test all time warp cases
 
 
 def test_num_routes_calculation():
     data = read("data/OkSmall.txt")
     data = make_heterogeneous(
         data, vehicle_types=[VehicleType(10, 2), VehicleType(20, 1)]
@@ -503,15 +632,15 @@
     "vehicle_types",
     [[VehicleType(10, 3)], [VehicleType(10, 2), VehicleType(20, 1)]],
 )
 def test_str_contains_routes(vehicle_types):
     data = read("data/OkSmall.txt")
     data = make_heterogeneous(data, vehicle_types)
 
-    rng = XorShift128(seed=2)
+    rng = RandomNumberGenerator(seed=2)
 
     for _ in range(5):  # let's do this a few times to really make sure
         sol = Solution.make_random(data, rng)
         str_representation = str(sol).splitlines()
         routes = sol.get_routes()
 
         # There should be no more than len(routes) lines (each detailing a
@@ -523,15 +652,15 @@
         for route, str_route in zip(routes, str_representation):
             for client in route:
                 assert_(str(client) in str_route)
 
 
 def test_hash():
     data = read("data/OkSmall.txt")
-    rng = XorShift128(seed=2)
+    rng = RandomNumberGenerator(seed=2)
 
     sol1 = Solution.make_random(data, rng)
     sol2 = Solution.make_random(data, rng)
 
     hash1 = hash(sol1)
     hash2 = hash(sol2)
 
@@ -552,9 +681,9 @@
     x = np.array([data.client(client).x for client in range(5)])
     y = np.array([data.client(client).y for client in range(5)])
 
     routes = [Route(data, [1, 2], 0), Route(data, [3], 0), Route(data, [4], 0)]
 
     for route in routes:
         x_center, y_center = route.centroid()
-        assert_equal(x_center, x[route].mean())
-        assert_equal(y_center, y[route].mean())
+        assert_allclose(x_center, x[route].mean())
+        assert_allclose(y_center, y[route].mean())
```

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_Statistics.py` & `pyvrp-0.5.0/pyvrp/tests/test_Statistics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from numpy.testing import assert_, assert_equal
 
-from pyvrp import CostEvaluator, Population, Statistics, XorShift128
+from pyvrp import CostEvaluator, Population, RandomNumberGenerator, Statistics
 from pyvrp.diversity import broken_pairs_distance
 from pyvrp.tests.helpers import make_random_solutions, read
 
 
 def test_csv_serialises_correctly(tmp_path):
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=42)
+    rng = RandomNumberGenerator(seed=42)
     pop = Population(broken_pairs_distance)
 
     for sol in make_random_solutions(10, data, rng):
         pop.add(sol, cost_evaluator)
 
     collected_stats = Statistics()
```

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_SubPopulation.py` & `pyvrp-0.5.0/pyvrp/tests/test_SubPopulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import numpy as np
 from numpy.testing import assert_, assert_allclose, assert_equal
 from pytest import mark
 
-from pyvrp import CostEvaluator, PopulationParams, Solution, XorShift128
+from pyvrp import (
+    CostEvaluator,
+    PopulationParams,
+    RandomNumberGenerator,
+    Solution,
+)
 from pyvrp._pyvrp import SubPopulation
 from pyvrp.diversity import broken_pairs_distance as bpd
 from pyvrp.tests.helpers import read
 
 
 @mark.parametrize("nb_close", [5, 10, 25])
 def test_avg_distance_closest_is_same_up_to_nb_close(nb_close: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=5)
+    rng = RandomNumberGenerator(seed=5)
 
     params = PopulationParams(
         min_pop_size=0, generation_size=250, nb_close=nb_close
     )
 
     subpop = SubPopulation(bpd, params)
     assert_equal(len(subpop), 0)
@@ -75,15 +80,15 @@
         distances = np.array([item.avg_distance_closest() for item in subpop])
         assert_allclose(distances, distances.mean())
 
 
 def test_fitness_is_purely_based_on_cost_when_only_elites():
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=51)
+    rng = RandomNumberGenerator(seed=51)
     params = PopulationParams(nb_elite=25, min_pop_size=25)
     subpop = SubPopulation(bpd, params)
 
     for _ in range(params.min_pop_size):
         subpop.add(Solution.make_random(data, rng), cost_evaluator)
 
     # We need to call update_fitness before accessing the fitness
@@ -100,22 +105,22 @@
     rank[by_cost] = np.arange(len(subpop))
 
     expected_fitness = rank / (2 * len(subpop))
     actual_fitness = np.array([item.fitness for item in subpop])
 
     # The fitness terms should all be bounded to [0, 1], and the values should
     # agree with what we've computed above.
-    assert_(((0 <= actual_fitness) & (actual_fitness <= 1)).all())
+    assert_(((actual_fitness >= 0) & (actual_fitness <= 1)).all())
     assert_allclose(actual_fitness, expected_fitness)
 
 
 def test_fitness_is_average_of_cost_and_diversity_when_no_elites():
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
-    rng = XorShift128(seed=52)
+    rng = RandomNumberGenerator(seed=52)
     params = PopulationParams(nb_elite=0, min_pop_size=25)
     subpop = SubPopulation(bpd, params)
 
     for _ in range(params.min_pop_size):
         subpop.add(Solution.make_random(data, rng), cost_evaluator)
 
     # We need to call update_fitness before accessing the fitness
@@ -136,9 +141,9 @@
     ranks[cost_rank[div_rank], 1] = np.arange(len(subpop))
 
     expected_fitness = ranks.sum(axis=1) / (2 * len(subpop))
     actual_fitness = np.array([item.fitness for item in subpop])
 
     # The fitness terms should all be bounded to [0, 1], and the values should
     # agree with what we've computed above.
-    assert_(((0 <= actual_fitness) & (actual_fitness <= 1)).all())
+    assert_(((actual_fitness >= 0) & (actual_fitness <= 1)).all())
     assert_allclose(actual_fitness, expected_fitness)
```

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_TimeWindowSegment.py` & `pyvrp-0.5.0/pyvrp/tests/test_TimeWindowSegment.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/pyvrp/tests/test_read.py` & `pyvrp-0.5.0/pyvrp/tests/test_read.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,38 +2,34 @@
 from pytest import mark
 
 from pyvrp.exceptions import ScalingWarning
 from pyvrp.tests.helpers import read
 
 
 @mark.parametrize(
-    "where, exception",
+    ("where", "exception"),
     [
         ("data/UnknownEdgeWeightFmt.txt", ValueError),
         ("data/UnknownEdgeWeightType.txt", ValueError),
         ("somewhere that does not exist", FileNotFoundError),
         ("data/FileWithUnknownSection.txt", ValueError),
         ("data/DepotNotOne.txt", ValueError),
         ("data/MoreThanOneDepot.txt", ValueError),
-        ("data/NonZeroDepotServiceDuration.txt", ValueError),
-        ("data/NonZeroDepotOpenTimeWindow.txt", ValueError),
-        ("data/NonZeroDepotReleaseTime.txt", ValueError),
-        ("data/NonZeroDepotDemand.txt", ValueError),
         ("data/TimeWindowOpenLargerThanClose.txt", ValueError),
         ("data/EdgeWeightsNoExplicit.txt", ValueError),
         ("data/EdgeWeightsNotFullMatrix.txt", ValueError),
     ],
 )
 def test_raises_invalid_file(where: str, exception: Exception):
     with assert_raises(exception):
         read(where)
 
 
 def test_raises_unknown_round_func():
-    with assert_raises(ValueError):
+    with assert_raises(TypeError):
         # Unknown round_func, so should raise.
         read("data/OkSmall.txt", round_func="asdbsadfas")
 
     # Is the default round_func, so should not raise.
     read("data/OkSmall.txt", round_func="none")
 
 
@@ -104,16 +100,16 @@
 def test_reading_En22k4_instance():  # instance from CVRPLIB
     data = read("data/E-n22-k4.txt", round_func="trunc1")
 
     assert_equal(data.num_clients, 21)
     assert_equal(data.vehicle_type(0).capacity, 6_000)
 
     # Coordinates are scaled by 10 to align with 1 decimal distance precision
-    assert_equal(data.depot().x, 1450)  # depot [x, y] location
-    assert_equal(data.depot().y, 2150)
+    assert_equal(data.client(0).x, 1450)  # depot [x, y] location
+    assert_equal(data.client(0).y, 2150)
 
     assert_equal(data.client(1).x, 1510)  # first customer [x, y] location
     assert_equal(data.client(1).y, 2640)
 
     # The data file specifies distances as 2D Euclidean. We take that and
     # should compute integer equivalents with up to one decimal precision.
     # For depot -> first customer:
@@ -140,18 +136,18 @@
         "data/RC208.txt", instance_format="solomon", round_func="trunc1"
     )
 
     assert_equal(data.num_clients, 100)  # Excl. depot
     assert_equal(data.vehicle_type(0).capacity, 1_000)
 
     # Coordinates and times are scaled by 10 for 1 decimal distance precision
-    assert_equal(data.depot().x, 400)  # depot [x, y] location
-    assert_equal(data.depot().y, 500)
-    assert_equal(data.depot().tw_early, 0)
-    assert_equal(data.depot().tw_late, 9600)
+    assert_equal(data.client(0).x, 400)  # depot [x, y] location
+    assert_equal(data.client(0).y, 500)
+    assert_equal(data.client(0).tw_early, 0)
+    assert_equal(data.client(0).tw_late, 9600)
 
     # Note: everything except demand is scaled by 10
     assert_equal(data.client(1).x, 250)  # first customer [x, y] location
     assert_equal(data.client(1).y, 850)
     assert_equal(data.client(1).demand, 20)
     assert_equal(data.client(1).tw_early, 3880)
     assert_equal(data.client(1).tw_late, 9110)
```

### Comparing `pyvrp-0.4.4/subprojects/pybind11.wrap` & `pyvrp-0.5.0/subprojects/pybind11.wrap`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.4/PKG-INFO` & `pyvrp-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvrp
-Version: 0.4.4
+Version: 0.5.0
 Summary: A state-of-the-art vehicle routing problem solver.
 Home-page: https://github.com/PyVRP/PyVRP
 License: MIT
 Author: Niels Wouda
 Author-email: nielswouda@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,46 +23,54 @@
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: vrplib (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/PyVRP/PyVRP
 Project-URL: Tracker, https://github.com/PyVRP/PyVRP/issues
 Description-Content-Type: text/markdown
 
-![PyVRP logo](docs/source/assets/images/PyVRP.svg)
+![PyVRP logo](docs/source/assets/images/logo.svg)
 
 [![PyPI version](https://badge.fury.io/py/pyvrp.svg)](https://badge.fury.io/py/pyvrp)
 [![CI](https://github.com/PyVRP/PyVRP/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/PyVRP/PyVRP/actions/workflows/CI.yml)
-[![Documentation Status](https://readthedocs.org/projects/pyvrp/badge/?version=latest)](https://pyvrp.readthedocs.io/en/latest/?badge=latest)
+[![DOC](https://github.com/PyVRP/PyVRP/actions/workflows/DOC.yml/badge.svg?branch=main)](https://pyvrp.org/)
 [![codecov](https://codecov.io/gh/PyVRP/PyVRP/branch/main/graph/badge.svg?token=G9JKIVZOHB)](https://codecov.io/gh/PyVRP/PyVRP)
 
-The `pyvrp` package is an open-source, state-of-the-art vehicle routing problem (VRP) solver.
-It currently supports the capacitated VRP (CVRP), the VRP with time windows (VRPTW), and prize-collecting. 
+PyVRP is an open-source, state-of-the-art vehicle routing problem (VRP) solver.
+It currently supports VRPs with:
+- Client demands (capacitated VRP);
+- Vehicles of different capacities;
+- Time windows, client service durations, and release times (VRP with time windows and release times);
+- Optional clients with prizes for visiting (prize collecting).
 
 The implementation builds on Thibaut Vidal's [HGS-CVRP][8], but has been completely redesigned to be easy to use as a highly customisable Python package, while maintaining speed and state-of-the-art performance.
 Users can customise various aspects of the algorithm using Python, including population management, crossover strategies, granular neighbourhoods and operator selection in the local search.
-Additionally, for advanced use cases such as supporting additional VRP variants, users can build and install `pyvrp` directly from the source code.
+Additionally, for advanced use cases such as supporting additional VRP variants, users can build and install PyVRP directly from the source code.
 
-`pyvrp` may be installed in the usual way as
+PyVRP is available on the Python package index as `pyvrp`.
+It may be installed in the usual way as
 ```
 pip install pyvrp
 ```
-This also resolves the few core dependencies `pyvrp` has.
+This also resolves the few core dependencies PyVRP has.
 The documentation is available [here][1].
 
 > If you are new to vehicle routing or metaheuristics, you might benefit from first reading the [introduction to VRP][6] and [introduction to HGS][7] pages.
 
 ### Examples
 
-We provide some example notebooks that show how the `pyvrp` package may be used to solve vehicle routing problems.
+We provide some example notebooks that show how PyVRP may be used to solve vehicle routing problems.
 These include:
 
-- The vehicle routing problem with time windows (VRPTW), [here][4].
-  We solve several instances from the literature, including a large 1000 customer instance.
-- The capacitated vehicle routing problem (CVRP), [here][5].
-  We solve an instance with 439 customers to near optimality within 30 seconds.
+- A short tutorial and introduction to PyVRP's modelling interface, [here][5].
+  This is a great way to get started with PyVRP.
+- A notebook solving classical VRP variants, [here][4].
+  In this notebook we solve several benchmark instances of the CVRP and VRPTW problems.
+  We also demonstrate how to use the plotting tools available in PyVRP to visualise the instance and statistics collected during the search procedure. 
+- A notebook implementing a `solve` method using PyVRP's components, [here][9].
+  This notebook is a great way to dive deeper into how PyVRP works internally.
 
 ### Contributing
 
 We are very grateful for any contributions you are willing to make. Please have
 a look [here][2] to get started. If you aim to make a large change, it is
 helpful to discuss the change first in a new GitHub issue. Feel free to open
 one!
@@ -72,23 +80,25 @@
 If you are looking for help, please follow the instructions [here][3].
 
 ### How to cite PyVRP
 
 TODO
 
 
-[1]: https://pyvrp.readthedocs.io/en/latest/
+[1]: https://pyvrp.org/
 
-[2]: https://pyvrp.readthedocs.io/en/latest/dev/contributing.html
+[2]: https://pyvrp.org/dev/contributing.html
 
-[3]: https://pyvrp.readthedocs.io/en/latest/setup/getting_help.html
+[3]: https://pyvrp.org/setup/getting_help.html
 
-[4]: https://pyvrp.readthedocs.io/en/latest/examples/vrptw.html
+[4]: https://pyvrp.org/examples/basic_vrps.html
 
-[5]: https://pyvrp.readthedocs.io/en/latest/examples/cvrp.html
+[5]: https://pyvrp.org/examples/quick_tutorial.html
 
-[6]: https://pyvrp.readthedocs.io/en/latest/setup/introduction_to_vrp.html
+[6]: https://pyvrp.org/setup/introduction_to_vrp.html
 
-[7]: https://pyvrp.readthedocs.io/en/latest/setup/introduction_to_hgs.html
+[7]: https://pyvrp.org/setup/introduction_to_hgs.html
 
 [8]: https://github.com/vidalt/HGS-CVRP/
 
+[9]: https://pyvrp.org/examples/using_pyvrp_components.html
+
```

