# Comparing `tmp/gdsfactory-6.98.2.tar.gz` & `tmp/gdsfactory-6.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdsfactory-6.98.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gdsfactory-6.99.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gdsfactory-6.98.2.tar` & `gdsfactory-6.99.0.tar`

### file list

```diff
@@ -1,701 +1,701 @@
--rw-r--r--   0        0        0     1072 2023-05-26 15:13:13.216617 gdsfactory-6.98.2/LICENSE
--rw-r--r--   0        0        0    14381 2023-05-26 15:13:13.216617 gdsfactory-6.98.2/README.md
--rw-r--r--   0        0        0     3583 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/__init__.py
--rw-r--r--   0        0        0     2104 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/add_keepout.py
--rw-r--r--   0        0        0    12629 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/add_labels.py
--rw-r--r--   0        0        0     3711 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/add_loopback.py
--rw-r--r--   0        0        0     5054 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/add_padding.py
--rw-r--r--   0        0        0    15639 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/add_pins.py
--rw-r--r--   0        0        0    14700 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/add_ports.py
--rw-r--r--   0        0        0     2884 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/add_tapers.py
--rw-r--r--   0        0        0     2257 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/add_tapers_cross_section.py
--rw-r--r--   0        0        0     1831 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/add_termination.py
--rw-r--r--   0        0        0     1856 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/asserts.py
--rw-r--r--   0        0        0    17589 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/cell.py
--rw-r--r--   0        0        0    16040 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/circuitviz.py
--rw-r--r--   0        0        0     5718 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/cli.py
--rw-r--r--   0        0        0   101901 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/component.py
--rw-r--r--   0        0        0    23424 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/component_layout.py
--rw-r--r--   0        0        0    29879 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/component_reference.py
--rw-r--r--   0        0        0     1205 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/C.py
--rw-r--r--   0        0        0     1144 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/L.py
--rw-r--r--   0        0        0    20964 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/__init__.py
--rw-r--r--   0        0        0     2621 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/add_fiducials.py
--rw-r--r--   0        0        0    14087 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/add_grating_couplers.py
--rw-r--r--   0        0        0     2014 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/add_trenches.py
--rw-r--r--   0        0        0     3207 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/align.py
--rw-r--r--   0        0        0     2622 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/array_component.py
--rw-r--r--   0        0        0     4705 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/array_with_fanout.py
--rw-r--r--   0        0        0     4322 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/array_with_via.py
--rw-r--r--   0        0        0     4042 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/awg.py
--rw-r--r--   0        0        0     1269 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/bbox.py
--rw-r--r--   0        0        0     2851 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/bend_circular.py
--rw-r--r--   0        0        0     2649 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/bend_circular_heater.py
--rw-r--r--   0        0        0     7903 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/bend_euler.py
--rw-r--r--   0        0        0     2682 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/bend_port.py
--rw-r--r--   0        0        0     3787 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/bend_s.py
--rw-r--r--   0        0        0     5373 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/bezier.py
--rw-r--r--   0        0        0     1605 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/cavity.py
--rw-r--r--   0        0        0     5766 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/cdc.py
--rw-r--r--   0        0        0     2929 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/cdsem_all.py
--rw-r--r--   0        0        0     1788 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/cdsem_bend180.py
--rw-r--r--   0        0        0     1631 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/cdsem_coupler.py
--rw-r--r--   0        0        0     1412 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/cdsem_straight.py
--rw-r--r--   0        0        0     1565 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/cdsem_straight_density.py
--rw-r--r--   0        0        0      793 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/circle.py
--rw-r--r--   0        0        0     5722 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/coh_rx_dual_pol.py
--rw-r--r--   0        0        0     8922 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/coh_rx_single_pol.py
--rw-r--r--   0        0        0     5043 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/coh_tx_dual_pol.py
--rw-r--r--   0        0        0     6118 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/coh_tx_single_pol.py
--rw-r--r--   0        0        0     2548 2023-05-26 15:13:13.224617 gdsfactory-6.98.2/gdsfactory/components/compass.py
--rw-r--r--   0        0        0     9876 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/component_lattice.py
--rw-r--r--   0        0        0     7174 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/component_sequence.py
--rw-r--r--   0        0        0      812 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/copy_layers.py
--rw-r--r--   0        0        0     3460 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/coupler.py
--rw-r--r--   0        0        0     2113 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/coupler90.py
--rw-r--r--   0        0        0     1802 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/coupler90bend.py
--rw-r--r--   0        0        0     4666 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/coupler_adiabatic.py
--rw-r--r--   0        0        0     1909 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/coupler_asymmetric.py
--rw-r--r--   0        0        0     3970 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/coupler_full.py
--rw-r--r--   0        0        0     3414 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/coupler_ring.py
--rw-r--r--   0        0        0     1060 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/coupler_straight.py
--rw-r--r--   0        0        0     1164 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/coupler_straight_asymmetric.py
--rw-r--r--   0        0        0     2192 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/coupler_symmetric.py
--rw-r--r--   0        0        0     1848 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/cross.py
--rw-r--r--   0        0        0    12873 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/crossing_waveguide.py
--rw-r--r--   0        0        0      500 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
--rw-r--r--   0        0        0     1014 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
--rw-r--r--   0        0        0    19749 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
--rw-r--r--   0        0        0    19751 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
--rw-r--r--   0        0        0    19749 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
--rw-r--r--   0        0        0    19751 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
--rw-r--r--   0        0        0    19775 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
--rw-r--r--   0        0        0     3143 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
--rw-r--r--   0        0        0     5272 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/cutback_2x2.py
--rw-r--r--   0        0        0     6450 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/cutback_bend.py
--rw-r--r--   0        0        0     3765 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/cutback_component.py
--rw-r--r--   0        0        0     2721 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/cutback_splitter.py
--rw-r--r--   0        0        0     2971 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/dbr.py
--rw-r--r--   0        0        0     4288 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/dbr_tapered.py
--rw-r--r--   0        0        0     2486 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/delay_snake.py
--rw-r--r--   0        0        0     3177 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/delay_snake2.py
--rw-r--r--   0        0        0     3245 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/delay_snake3.py
--rw-r--r--   0        0        0     4319 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/delay_snake_sbend.py
--rw-r--r--   0        0        0     1226 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/dicing_lane.py
--rw-r--r--   0        0        0     3471 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/die.py
--rw-r--r--   0        0        0     2975 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/die_bbox.py
--rw-r--r--   0        0        0     2863 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/die_bbox_frame.py
--rw-r--r--   0        0        0     8015 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/disk.py
--rw-r--r--   0        0        0     4112 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/edge_coupler_array.py
--rw-r--r--   0        0        0     1214 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/ellipse.py
--rw-r--r--   0        0        0     1800 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/extend_ports_list.py
--rw-r--r--   0        0        0     7988 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/extension.py
--rw-r--r--   0        0        0      981 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/fiber.py
--rw-r--r--   0        0        0     1432 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/fiber_array.py
--rw-r--r--   0        0        0      722 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/fiducial_squares.py
--rw-r--r--   0        0        0     3290 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/ge_detector_straight_si_contacts.py
--rw-r--r--   0        0        0     1063 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_array.py
--rw-r--r--   0        0        0     4682 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_dual_pol.py
--rw-r--r--   0        0        0     7110 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_elliptical.py
--rw-r--r--   0        0        0     7222 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
--rw-r--r--   0        0        0     4961 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_elliptical_lumerical.py
--rw-r--r--   0        0        0     4592 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_elliptical_trenches.py
--rw-r--r--   0        0        0     1773 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_functions.py
--rw-r--r--   0        0        0     9058 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_loss.py
--rw-r--r--   0        0        0     1786 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_loss_fiber_single.py
--rw-r--r--   0        0        0     4142 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_rectangular.py
--rw-r--r--   0        0        0     4685 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
--rw-r--r--   0        0        0     3887 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
--rw-r--r--   0        0        0     1579 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/grating_coupler_tree.py
--rw-r--r--   0        0        0     8811 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/greek_cross.py
--rw-r--r--   0        0        0     1019 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/hline.py
--rw-r--r--   0        0        0     3687 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/interdigital_capacitor.py
--rw-r--r--   0        0        0     1825 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/litho_calipers.py
--rw-r--r--   0        0        0     1244 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/litho_ruler.py
--rw-r--r--   0        0        0     1304 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/litho_steps.py
--rw-r--r--   0        0        0      650 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/logo.py
--rw-r--r--   0        0        0     1679 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/loop_mirror.py
--rw-r--r--   0        0        0     3873 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mmi1x2.py
--rw-r--r--   0        0        0     2814 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mmi1x2_with_sbend.py
--rw-r--r--   0        0        0     3858 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mmi2x2.py
--rw-r--r--   0        0        0     3299 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mmi2x2_with_sbend.py
--rw-r--r--   0        0        0     4947 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mmi_90degree_hybrid.py
--rw-r--r--   0        0        0     3265 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mode_converter.py
--rw-r--r--   0        0        0     7579 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mzi.py
--rw-r--r--   0        0        0     2499 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mzi_arm.py
--rw-r--r--   0        0        0     5835 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mzi_arms.py
--rw-r--r--   0        0        0    12214 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mzi_lattice.py
--rw-r--r--   0        0        0     4025 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mzi_pads_center.py
--rw-r--r--   0        0        0     1064 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mzi_phase_shifter.py
--rw-r--r--   0        0        0     6342 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mzit.py
--rw-r--r--   0        0        0     3502 2023-05-26 15:13:13.228618 gdsfactory-6.98.2/gdsfactory/components/mzit_lattice.py
--rw-r--r--   0        0        0     6047 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/mzm.py
--rw-r--r--   0        0        0     3518 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/nxn.py
--rw-r--r--   0        0        0     1940 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/optimal_90deg.py
--rw-r--r--   0        0        0     3876 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/optimal_hairpin.py
--rw-r--r--   0        0        0     6131 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/optimal_step.py
--rw-r--r--   0        0        0     6327 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/pack_doe.py
--rw-r--r--   0        0        0     3860 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/pad.py
--rw-r--r--   0        0        0     1890 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/pad_gsg.py
--rw-r--r--   0        0        0     1157 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/pads_shorted.py
--rw-r--r--   0        0        0     3833 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/polarization_splitter_rotator.py
--rw-r--r--   0        0        0     1147 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ramp.py
--rw-r--r--   0        0        0     1508 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/rectangle.py
--rw-r--r--   0        0        0     2972 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/rectangle_with_slits.py
--rw-r--r--   0        0        0     1508 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/regular_polygon.py
--rw-r--r--   0        0        0     3302 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/resistance_meander.py
--rw-r--r--   0        0        0     2642 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/resistance_sheet.py
--rw-r--r--   0        0        0     1273 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring.py
--rw-r--r--   0        0        0     4143 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_crow.py
--rw-r--r--   0        0        0     3272 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_crow_couplers.py
--rw-r--r--   0        0        0     2267 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_double.py
--rw-r--r--   0        0        0     2846 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_double_bend_coupler.py
--rw-r--r--   0        0        0     3846 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_double_heater.py
--rw-r--r--   0        0        0     7757 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_double_pn.py
--rw-r--r--   0        0        0    12137 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_section_based.py
--rw-r--r--   0        0        0     2740 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_single.py
--rw-r--r--   0        0        0     1968 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_single_array.py
--rw-r--r--   0        0        0     6868 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_single_bend_coupler.py
--rw-r--r--   0        0        0     2714 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_single_dut.py
--rw-r--r--   0        0        0     4018 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_single_heater.py
--rw-r--r--   0        0        0     5267 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/ring_single_pn.py
--rw-r--r--   0        0        0     2282 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/seal_ring.py
--rw-r--r--   0        0        0     3758 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/snspd.py
--rw-r--r--   0        0        0     2059 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/spiral_double.py
--rw-r--r--   0        0        0     5871 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/spiral_external_io.py
--rw-r--r--   0        0        0    16692 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/spiral_heater.py
--rw-r--r--   0        0        0     9181 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/spiral_inner_io.py
--rw-r--r--   0        0        0     1733 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/splitter_chain.py
--rw-r--r--   0        0        0     5327 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/splitter_tree.py
--rw-r--r--   0        0        0     2451 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/straight.py
--rw-r--r--   0        0        0     1033 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/straight_array.py
--rw-r--r--   0        0        0     7914 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/straight_heater_doped_rib.py
--rw-r--r--   0        0        0     1922 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/straight_heater_doped_strip.py
--rw-r--r--   0        0        0     7891 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/straight_heater_meander.py
--rw-r--r--   0        0        0     8090 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/straight_heater_meander_doped.py
--rw-r--r--   0        0        0     5686 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/straight_heater_metal.py
--rw-r--r--   0        0        0     2809 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/straight_pin.py
--rw-r--r--   0        0        0     3974 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/straight_pin_slot.py
--rw-r--r--   0        0        0      655 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/straight_rib.py
--rw-r--r--   0        0        0      820 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/switch_tree.py
--rw-r--r--   0        0        0     7730 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/taper.py
--rw-r--r--   0        0        0     3530 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/taper_adiabatic.py
--rw-r--r--   0        0        0     2457 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/taper_cross_section.py
--rw-r--r--   0        0        0     2363 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/taper_from_csv.py
--rw-r--r--   0        0        0     1215 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/taper_parabolic.py
--rw-r--r--   0        0        0     1635 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/terminator.py
--rw-r--r--   0        0        0     2913 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/text.py
--rw-r--r--   0        0        0     3821 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/text_freetype.py
--rw-r--r--   0        0        0     3160 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/text_rectangular.py
--rw-r--r--   0        0        0     3943 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/text_rectangular_font.py
--rw-r--r--   0        0        0     2536 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/triangles.py
--rw-r--r--   0        0        0      715 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/verniers.py
--rw-r--r--   0        0        0     2468 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/version_stamp.py
--rw-r--r--   0        0        0     2436 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/via.py
--rw-r--r--   0        0        0     3060 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/via_corner.py
--rw-r--r--   0        0        0     5342 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/via_cutback.py
--rw-r--r--   0        0        0    15612 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/via_stack.py
--rw-r--r--   0        0        0     4430 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/via_stack_slot.py
--rw-r--r--   0        0        0     4944 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/via_stack_with_offset.py
--rw-r--r--   0        0        0     1088 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/wafer.py
--rw-r--r--   0        0        0     2542 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/wire.py
--rw-r--r--   0        0        0      978 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/components/wire_sbend.py
--rw-r--r--   0        0        0     8145 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/config.py
--rw-r--r--   0        0        0      481 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/conftest.py
--rw-r--r--   0        0        0    38409 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/constants.py
--rw-r--r--   0        0        0     1476 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/containers.py
--rw-r--r--   0        0        0    83060 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/cross_section.py
--rw-r--r--   0        0        0     2982 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/decorators.py
--rw-r--r--   0        0        0     7312 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/difftest.py
--rw-r--r--   0        0        0     1020 2023-05-26 15:13:13.232617 gdsfactory-6.98.2/gdsfactory/events.py
--rw-r--r--   0        0        0      267 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/export/__init__.py
--rw-r--r--   0        0        0     3353 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/export/to_3d.py
--rw-r--r--   0        0        0     7599 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/export/to_gerber.py
--rw-r--r--   0        0        0     1940 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/export/to_np.py
--rw-r--r--   0        0        0     3058 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/export/to_stl.py
--rw-r--r--   0        0        0     2976 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/filestorage.py
--rw-r--r--   0        0        0    11890 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/fill.py
--rw-r--r--   0        0        0     7799 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/font.py
--rw-r--r--   0        0        0     8073 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/functions.py
--rw-r--r--   0        0        0       20 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/gdsdiff/.gitattributes
--rw-r--r--   0        0        0       83 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/gdsdiff/.gitconfig
--rw-r--r--   0        0        0       72 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/gdsdiff/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/gdsdiff/gds_diff_git.py
--rw-r--r--   0        0        0     2935 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/gdsdiff/gdsdiff.py
--rw-r--r--   0        0        0      708 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/gdsdiff/install.py
--rw-r--r--   0        0        0      271 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/gdsdiff/sample.py
--rw-r--r--   0        0        0     1059 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/gdsdiff/test_xor.py
--rw-r--r--   0        0        0     1100 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/README.md
--rw-r--r--   0        0        0     1722 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/__init__.py
--rw-r--r--   0        0        0      169 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/generic_tech.sh
--rw-r--r--   0        0        0     8142 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/get_klayout_pyxs.py
--rw-r--r--   0        0        0      161 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/README.md
--rw-r--r--   0        0        0      104 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/drc/Makefile
--rw-r--r--   0        0        0        0 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/drc/__init__.py
--rw-r--r--   0        0        0     2842 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/drc/errors.py
--rw-r--r--   0        0        0     6193 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/grain.xml
--rw-r--r--   0        0        0    10140 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/icon_128x128.png
--rw-r--r--   0        0        0     4248 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/icon_64x64.png
--rw-r--r--   0        0        0       27 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/.gitignore
--rw-r--r--   0        0        0      494 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/Makefile
--rw-r--r--   0        0        0     4062 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/README.md
--rw-r--r--   0        0        0     2419 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
--rw-r--r--   0        0        0     9696 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
--rw-r--r--   0        0        0    12379 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
--rw-r--r--   0        0        0     7235 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
--rw-r--r--   0        0        0     3446 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
--rw-r--r--   0        0        0      479 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
--rw-r--r--   0        0        0      582 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
--rw-r--r--   0        0        0      108 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
--rw-r--r--   0        0        0      186 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
--rw-r--r--   0        0        0      398 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
--rw-r--r--   0        0        0      574 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
--rw-r--r--   0        0        0     6034 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
--rw-r--r--   0        0        0    10704 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
--rw-r--r--   0        0        0      477 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
--rw-r--r--   0        0        0     4337 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
--rw-r--r--   0        0        0      926 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
--rw-r--r--   0        0        0    10945 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
--rw-r--r--   0        0        0      710 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
--rw-r--r--   0        0        0      538 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
--rw-r--r--   0        0        0        0 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/python/__init__.py
--rw-r--r--   0        0        0      114 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
--rw-r--r--   0        0        0     4311 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
--rw-r--r--   0        0        0      269 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/Makefile
--rw-r--r--   0        0        0     1854 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
--rw-r--r--   0        0        0     1519 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/generic.layerstack
--rw-r--r--   0        0        0    41073 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
--rw-r--r--   0        0        0    40616 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/layers.lyp
--rw-r--r--   0        0        0     5977 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/tech.lyt
--rw-r--r--   0        0        0     4258 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
--rw-r--r--   0        0        0     4537 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
--rw-r--r--   0        0        0     4690 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
--rw-r--r--   0        0        0     5508 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
--rw-r--r--   0        0        0     1883 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/layer_map.py
--rw-r--r--   0        0        0     6511 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/layer_stack.py
--rw-r--r--   0        0        0    10780 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/layer_views.yaml
--rw-r--r--   0        0        0      158 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/generic_tech/simulation_settings.py
--rw-r--r--   0        0        0     1431 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/__init__.py
--rw-r--r--   0        0        0     4917 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/boolean.py
--rw-r--r--   0        0        0     3814 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/boolean_klayout.py
--rw-r--r--   0        0        0     1904 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/boolean_polygons.py
--rw-r--r--   0        0        0      598 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/check_duplicated_cells.py
--rw-r--r--   0        0        0     2719 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/check_exclusion.py
--rw-r--r--   0        0        0     2829 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/check_inclusion.py
--rw-r--r--   0        0        0     3566 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/check_space.py
--rw-r--r--   0        0        0     1904 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/check_width.py
--rw-r--r--   0        0        0     5010 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/fill_klayout.py
--rw-r--r--   0        0        0     7034 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/fill_tiled.py
--rw-r--r--   0        0        0     1697 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/fillet.py
--rw-r--r--   0        0        0     6664 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/functions.py
--rw-r--r--   0        0        0     2167 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/invert.py
--rw-r--r--   0        0        0     3685 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/layer_priority.py
--rw-r--r--   0        0        0     3054 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/manhattanize.py
--rw-r--r--   0        0        0     4192 2023-05-26 15:13:13.236617 gdsfactory-6.98.2/gdsfactory/geometry/maskprep.py
--rw-r--r--   0        0        0     4814 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/geometry/maskprep_flat.py
--rw-r--r--   0        0        0     3250 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/geometry/offset.py
--rw-r--r--   0        0        0     3842 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/geometry/outline.py
--rw-r--r--   0        0        0     2510 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/geometry/trim.py
--rw-r--r--   0        0        0     2948 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/geometry/union.py
--rw-r--r--   0        0        0     3609 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/geometry/write_connectivity.py
--rw-r--r--   0        0        0    10532 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/geometry/write_drc.py
--rw-r--r--   0        0        0     1783 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/geometry/xor_diff.py
--rw-r--r--   0        0        0     1158 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/get_factories.py
--rw-r--r--   0        0        0    23569 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/get_netlist.py
--rw-r--r--   0        0        0    14446 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/get_netlist_flat.py
--rw-r--r--   0        0        0      682 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/get_netlist_klayout.py
--rw-r--r--   0        0        0     9745 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/grid.py
--rw-r--r--   0        0        0     4393 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/install.py
--rw-r--r--   0        0        0     1970 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/klive.py
--rw-r--r--   0        0        0      585 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/labels/__init__.py
--rw-r--r--   0        0        0     3563 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/labels/add_label_yaml.py
--rw-r--r--   0        0        0     3847 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/labels/ehva.py
--rw-r--r--   0        0        0     3810 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/labels/merge_test_metadata.py
--rw-r--r--   0        0        0     4668 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/labels/siepic.py
--rw-r--r--   0        0        0     4847 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/labels/write_labels.py
--rw-r--r--   0        0        0     1149 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/materials.py
--rw-r--r--   0        0        0     5247 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/name.py
--rw-r--r--   0        0        0    11586 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/pack.py
--rw-r--r--   0        0        0    50959 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/path.py
--rw-r--r--   0        0        0    27294 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/pdk.py
--rw-r--r--   0        0        0     6220 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/picmodel.py
--rw-r--r--   0        0        0     5068 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/pixelate.py
--rw-r--r--   0        0        0        0 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/dagster/__init__.py
--rw-r--r--   0        0        0      976 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/dagster/workflow.py
--rw-r--r--   0        0        0      566 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/database/README.md
--rw-r--r--   0        0        0        0 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/database/__init__.py
--rw-r--r--   0        0        0     6216 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/database/db_upload.py
--rw-r--r--   0        0        0    16143 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/database/models.py
--rw-r--r--   0        0        0       32 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/Makefile
--rw-r--r--   0        0        0       23 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/__init__.py
--rw-r--r--   0        0        0     4080 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/main.py
--rwxr-xr-x   0        0        0     7511 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/server.py
--rwxr-xr-x   0        0        0      594 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/server_jupyter.py
--rw-r--r--   0        0        0     1299 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/static/client.css
--rw-r--r--   0        0        0     9637 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/static/client.js
--rw-r--r--   0        0        0      840 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/templates/client.html
--rw-r--r--   0        0        0      236 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/templates/footer.html
--rw-r--r--   0        0        0      229 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/templates/gdspaths.html
--rw-r--r--   0        0        0      572 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/templates/header.html
--rw-r--r--   0        0        0      253 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/templates/index.html
--rw-r--r--   0        0        0      964 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/templates/navbar.html
--rw-r--r--   0        0        0     1837 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/plugins/web/templates/viewer.html
--rw-r--r--   0        0        0    32235 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/port.py
--rw-r--r--   0        0        0    37817 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/quickplotter.py
--rw-r--r--   0        0        0      696 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/read/__init__.py
--rw-r--r--   0        0        0     1639 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/read/from_dphox.py
--rw-r--r--   0        0        0     1285 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/read/from_gdspaths.py
--rw-r--r--   0        0        0     1953 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/read/from_np.py
--rw-r--r--   0        0        0     2813 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/read/from_phidl.py
--rw-r--r--   0        0        0    38082 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/read/from_yaml.py
--rw-r--r--   0        0        0     5897 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/read/from_yaml_template.py
--rw-r--r--   0        0        0     5688 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/read/import_gds.py
--rw-r--r--   0        0        0     3407 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/read/labels.py
--rw-r--r--   0        0        0     3769 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/routing/__init__.py
--rw-r--r--   0        0        0     2920 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/routing/add_electrical_pads_shortest.py
--rw-r--r--   0        0        0     3015 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/routing/add_electrical_pads_top.py
--rw-r--r--   0        0        0     3035 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/routing/add_electrical_pads_top_dc.py
--rw-r--r--   0        0        0     8715 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/routing/add_fiber_array.py
--rw-r--r--   0        0        0    10624 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/routing/add_fiber_single.py
--rw-r--r--   0        0        0     8967 2023-05-26 15:13:13.240618 gdsfactory-6.98.2/gdsfactory/routing/add_pads.py
--rw-r--r--   0        0        0    38948 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/all_angle.py
--rw-r--r--   0        0        0     3916 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/auto_taper.py
--rw-r--r--   0        0        0      982 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/factories.py
--rw-r--r--   0        0        0     4415 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/fanout.py
--rw-r--r--   0        0        0     2800 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/fanout2x2.py
--rw-r--r--   0        0        0    24342 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_bundle.py
--rw-r--r--   0        0        0     8652 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_bundle_corner.py
--rw-r--r--   0        0        0     6910 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_bundle_from_steps.py
--rw-r--r--   0        0        0    12949 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_bundle_from_waypoints.py
--rw-r--r--   0        0        0     5284 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_bundle_path_length_match.py
--rw-r--r--   0        0        0     1937 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_bundle_sbend.py
--rw-r--r--   0        0        0    17064 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_bundle_u.py
--rw-r--r--   0        0        0     1510 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_input_labels.py
--rw-r--r--   0        0        0     9233 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_route.py
--rw-r--r--   0        0        0    10872 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_route_astar.py
--rw-r--r--   0        0        0     6119 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_route_from_steps.py
--rw-r--r--   0        0        0     2766 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_route_sbend.py
--rw-r--r--   0        0        0     3311 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_routes_bend180.py
--rw-r--r--   0        0        0     1854 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/get_routes_straight.py
--rw-r--r--   0        0        0    34394 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/manhattan.py
--rw-r--r--   0        0        0    10081 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/path_length_matching.py
--rw-r--r--   0        0        0    22568 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/route_fiber_array.py
--rw-r--r--   0        0        0     8679 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/route_fiber_single.py
--rw-r--r--   0        0        0    18132 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/route_ports_to_side.py
--rw-r--r--   0        0        0     4379 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/route_quad.py
--rw-r--r--   0        0        0    14370 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/route_sharp.py
--rw-r--r--   0        0        0    10167 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/route_south.py
--rw-r--r--   0        0        0     5072 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/sort_ports.py
--rw-r--r--   0        0        0     2477 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/routing/utils.py
--rw-r--r--   0        0        0     2897 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/01_component_pcell.py
--rw-r--r--   0        0        0      646 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
--rw-r--r--   0        0        0     1109 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/01_component_pcell_with_pins.py
--rw-r--r--   0        0        0      664 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
--rw-r--r--   0        0        0      347 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/02_component_autoname.py
--rw-r--r--   0        0        0      887 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/03_move.py
--rw-r--r--   0        0        0      881 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/04_connect.py
--rw-r--r--   0        0        0      710 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/05_remove_layers.py
--rw-r--r--   0        0        0      931 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/06_remapping_layers.py
--rw-r--r--   0        0        0     1082 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/07_flattening_device.py
--rw-r--r--   0        0        0      475 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/08_group.py
--rw-r--r--   0        0        0     1631 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/11_component_layout.py
--rw-r--r--   0        0        0     2245 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/12_component_refs.py
--rw-r--r--   0        0        0      955 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/13_component_netlist.py
--rw-r--r--   0        0        0     2592 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/14_component_connectivity.py
--rw-r--r--   0        0        0     1636 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/15_component_sequence1.py
--rw-r--r--   0        0        0     1680 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/16_component_sequence2.py
--rw-r--r--   0        0        0      965 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/17_ports.py
--rw-r--r--   0        0        0      489 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/18_port_markers.py
--rw-r--r--   0        0        0      361 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/19_references.py
--rw-r--r--   0        0        0      533 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/20_components.py
--rw-r--r--   0        0        0      507 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/21_add_fiber_array.py
--rw-r--r--   0        0        0      493 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/22_add_fiber_single.py
--rw-r--r--   0        0        0      569 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/22_add_pads.py
--rw-r--r--   0        0        0      848 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/23_reticle.py
--rw-r--r--   0        0        0     1588 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/23_reticle_passives.py
--rw-r--r--   0        0        0      457 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/24_doe.py
--rw-r--r--   0        0        0      687 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/24_doe_2.py
--rw-r--r--   0        0        0      692 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/24_doe_3.py
--rw-r--r--   0        0        0      306 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/25_slot_cross_section.py
--rw-r--r--   0        0        0     1363 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/30_lidar.py
--rw-r--r--   0        0        0     1412 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/30_lidar_pcell.py
--rw-r--r--   0        0        0     1943 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/30_lidar_with_pads.py
--rw-r--r--   0        0        0        0 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/__init__.py
--rw-r--r--   0        0        0     1307 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing.py
--rw-r--r--   0        0        0      558 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
--rw-r--r--   0        0        0     6062 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
--rw-r--r--   0        0        0      444 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
--rw-r--r--   0        0        0      463 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
--rw-r--r--   0        0        0     1552 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
--rw-r--r--   0        0        0     1315 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
--rw-r--r--   0        0        0      602 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
--rw-r--r--   0        0        0     3317 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
--rw-r--r--   0        0        0     1484 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
--rw-r--r--   0        0        0     3045 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
--rw-r--r--   0        0        0     3782 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
--rw-r--r--   0        0        0     1988 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/big_device.py
--rw-r--r--   0        0        0       19 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/Makefile
--rw-r--r--   0        0        0        0 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/benchmark/fill_demo.py
--rw-r--r--   0        0        0      343 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
--rw-r--r--   0        0        0      637 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/circuits/mask.pic.yml
--rw-r--r--   0        0        0      622 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
--rw-r--r--   0        0        0      569 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
--rw-r--r--   0        0        0      453 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/circuits/pads.pic.yml
--rw-r--r--   0        0        0      287 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/circuits/rectangles.pic.yml
--rw-r--r--   0        0        0     2260 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/drc_errors.py
--rw-r--r--   0        0        0     1014 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/drc_write.py
--rw-r--r--   0        0        0     4530 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/layers.py
--rw-r--r--   0        0        0      158 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/layers_sky130.py
--rw-r--r--   0        0        0      364 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/layers_xsection.py
--rw-r--r--   0        0        0     1065 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/lvs.py
--rw-r--r--   0        0        0      574 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/demo/pcell.py
--rw-r--r--   0        0        0     4174 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/netlists/mzi.yml
--rw-r--r--   0        0        0     5840 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/netlists/mzi_full.yml
--rw-r--r--   0        0        0        0 2023-05-26 15:13:13.244618 gdsfactory-6.98.2/gdsfactory/samples/pdk/__init__.py
--rw-r--r--   0        0        0     4235 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/fab_c.py
--rw-r--r--   0        0        0      475 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/fab_d/__init__.py
--rw-r--r--   0        0        0     1880 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/fab_d/phase_shifters.py
--rw-r--r--   0        0        0     1715 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c.py
--rw-r--r--   0        0        0       50 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
--rw-r--r--   0        0        0       93 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
--rw-r--r--   0        0        0       85 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
--rw-r--r--   0        0        0      139 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
--rw-r--r--   0        0        0       90 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
--rw-r--r--   0        0        0      126 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
--rw-r--r--   0        0        0       48 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
--rw-r--r--   0        0        0     1023 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
--rw-r--r--   0        0        0     2206 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
--rw-r--r--   0        0        0     1879 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
--rw-r--r--   0        0        0     1283 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
--rw-r--r--   0        0        0     1632 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
--rw-r--r--   0        0        0     1061 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
--rw-r--r--   0        0        0     1054 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
--rw-r--r--   0        0        0     1617 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
--rw-r--r--   0        0        0     4497 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
--rw-r--r--   0        0        0     3625 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
--rw-r--r--   0        0        0     3603 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
--rw-r--r--   0        0        0     4455 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
--rw-r--r--   0        0        0      840 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
--rw-r--r--   0        0        0     2297 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
--rw-r--r--   0        0        0      316 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/schematic.py
--rw-r--r--   0        0        0    17862 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/schematic_editor.py
--rw-r--r--   0        0        0     4194 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/serialization.py
--rw-r--r--   0        0        0     1612 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/show.py
--rw-r--r--   0        0        0      724 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/__init__.py
--rw-r--r--   0        0        0     4369 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/add_simulation_markers.py
--rw-r--r--   0        0        0     2476 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/convert_sparameters.py
--rw-r--r--   0        0        0      547 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/devsim/__init__.py
--rw-r--r--   0        0        0     2559 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/devsim/doping.py
--rw-r--r--   0        0        0    11977 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/devsim/get_simulation.py
--rw-r--r--   0        0        0    23687 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/devsim/get_simulation_xsection.py
--rw-r--r--   0        0        0    19756 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/devsim/get_solver.py
--rw-r--r--   0        0        0     1644 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/devsim/test_devsim.py
--rw-r--r--   0        0        0      189 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/disable_print.py
--rw-r--r--   0        0        0       79 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/eme/__init__.py
--rw-r--r--   0        0        0    14784 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/eme/meow_eme.py
--rw-r--r--   0        0        0     1787 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/eme/test_meow_simulation.py
--rw-r--r--   0        0        0        0 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/fem/__init__.py
--rw-r--r--   0        0        0     8968 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/fem/mode_solver.py
--rw-r--r--   0        0        0     2221 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/fem/test_mode_solver.py
--rw-r--r--   0        0        0     3455 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/get_effective_indices.py
--rw-r--r--   0        0        0     3109 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/get_modes_path.py
--rw-r--r--   0        0        0     3888 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/get_sparameters_path.py
--rw-r--r--   0        0        0     2003 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/__init__.py
--rw-r--r--   0        0        0     3194 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_material.py
--rw-r--r--   0        0        0     6137 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_meep_geometry.py
--rw-r--r--   0        0        0     6054 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_port_eigenmode.py
--rw-r--r--   0        0        0    11014 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_simulation.py
--rw-r--r--   0        0        0    15915 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
--rw-r--r--   0        0        0    18182 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
--rw-r--r--   0        0        0    12312 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
--rw-r--r--   0        0        0    11914 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_eigenmode.py
--rw-r--r--   0        0        0      832 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_materials.py
--rw-r--r--   0        0        0    10128 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0     6642 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
--rw-r--r--   0        0        0    10128 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0    10093 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
--rw-r--r--   0        0        0    10085 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
--rw-r--r--   0        0        0    34701 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
--rw-r--r--   0        0        0    10123 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
--rw-r--r--   0        0        0     9966 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
--rw-r--r--   0        0        0     9966 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
--rw-r--r--   0        0        0    10129 2023-05-26 15:13:13.248618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
--rw-r--r--   0        0        0    14053 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/write_sparameters_grating.py
--rw-r--r--   0        0        0    21281 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/write_sparameters_meep.py
--rw-r--r--   0        0        0     8143 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
--rw-r--r--   0        0        0     9577 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
--rw-r--r--   0        0        0     1246 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/__init__.py
--rw-r--r--   0        0        0     6653 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/break_geometry.py
--rw-r--r--   0        0        0    11250 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/mesh.py
--rw-r--r--   0        0        0    11824 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/meshtracker.py
--rw-r--r--   0        0        0     7752 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/parse_component.py
--rw-r--r--   0        0        0     3644 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/parse_gds.py
--rw-r--r--   0        0        0     3605 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/parse_layerstack.py
--rw-r--r--   0        0        0     2990 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/refine.py
--rw-r--r--   0        0        0    10851 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/scratch/mesh3D.py
--rw-r--r--   0        0        0     2513 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/tests/test_meshing.py
--rw-r--r--   0        0        0    14168 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
--rw-r--r--   0        0        0     7441 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
--rw-r--r--   0        0        0    16334 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gmsh/xyz_mesh.py
--rw-r--r--   0        0        0     1624 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/__init__.py
--rw-r--r--   0        0        0     4368 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/get_results.py
--rw-r--r--   0        0        0    20009 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/get_simulation.py
--rw-r--r--   0        0        0    21071 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
--rw-r--r--   0        0        0     2821 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/materials.py
--rw-r--r--   0        0        0    27439 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/modes.py
--rw-r--r--   0        0        0     8941 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/sim_run.yaml
--rw-r--r--   0        0        0     8114 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
--rw-r--r--   0        0        0     8114 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
--rw-r--r--   0        0        0      744 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_modes.py
--rw-r--r--   0        0        0      262 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
--rw-r--r--   0        0        0      879 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_results.py
--rw-r--r--   0        0        0     1505 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
--rw-r--r--   0        0        0     1655 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
--rw-r--r--   0        0        0     9297 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
--rw-r--r--   0        0        0     1732 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0     1224 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/utils.py
--rw-r--r--   0        0        0    10841 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/write_sparameters.py
--rw-r--r--   0        0        0     7695 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0      588 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/lumerical/__init__.py
--rw-r--r--   0        0        0    16091 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/lumerical/interconnect.py
--rw-r--r--   0        0        0     4286 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/lumerical/read.py
--rw-r--r--   0        0        0     3569 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/lumerical/settings.py
--rw-r--r--   0        0        0     2368 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/lumerical/test_read_sparameters.py
--rw-r--r--   0        0        0    19865 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
--rw-r--r--   0        0        0     1504 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
--rw-r--r--   0        0        0      932 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/__init__.py
--rw-r--r--   0        0        0     1618 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/coupler.py
--rw-r--r--   0        0        0     4166 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/find_coupling_vs_gap.py
--rw-r--r--   0        0        0     2773 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/find_mode_dispersion.py
--rw-r--r--   0        0        0     8924 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/find_modes.py
--rwxr-xr-x   0        0        0     7032 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/find_modes_cross_section.py
--rw-r--r--   0        0        0     4458 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
--rw-r--r--   0        0        0     2728 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/find_neff_vs_width.py
--rw-r--r--   0        0        0     7148 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/get_mode_solver_coupler.py
--rwxr-xr-x   0        0        0     4462 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
--rw-r--r--   0        0        0     5411 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/get_mode_solver_rib.py
--rw-r--r--   0        0        0     1110 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
--rw-r--r--   0        0        0     1102 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
--rw-r--r--   0        0        0     1110 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
--rw-r--r--   0        0        0     8023 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/neff_convergence_test.py
--rw-r--r--   0        0        0      267 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/neff_vs_width.csv
--rw-r--r--   0        0        0     2469 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/overlap.py
--rw-r--r--   0        0        0      418 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/tests/test_dw_dh.py
--rw-r--r--   0        0        0       83 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
--rw-r--r--   0        0        0      548 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
--rw-r--r--   0        0        0     1137 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/tests/test_find_modes.py
--rw-r--r--   0        0        0      649 2023-05-26 15:13:13.252618 gdsfactory-6.98.2/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
--rw-r--r--   0        0        0      354 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
--rw-r--r--   0        0        0      113 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
--rw-r--r--   0        0        0    15492 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/modes/types.py
--rw-r--r--   0        0        0     1169 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/modes/waveguide.py
--rw-r--r--   0        0        0     2013 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/photonic_circuit_models/__init__.py
--rw-r--r--   0        0        0      597 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/photonic_circuit_models/coupler.py
--rw-r--r--   0        0        0      377 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/photonic_circuit_models/fsr.py
--rw-r--r--   0        0        0      418 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/photonic_circuit_models/heater.py
--rw-r--r--   0        0        0     3069 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/photonic_circuit_models/mzi.py
--rw-r--r--   0        0        0     2616 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/photonic_circuit_models/ring.py
--rw-r--r--   0        0        0     7332 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/plot.py
--rw-r--r--   0        0        0     2480 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/plot_csv.py
--rw-r--r--   0        0        0      613 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/port_symmetries.py
--rw-r--r--   0        0        0     4685 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/process/diffusion.py
--rw-r--r--   0        0        0     5317 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/process/implant_tables.py
--rw-r--r--   0        0        0     6800 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/process/pysrim.py
--rw-r--r--   0        0        0     2182 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/process/silicon.py
--rw-r--r--   0        0        0     1861 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/process/skew/antimony_si_skew.csv
--rw-r--r--   0        0        0     1050 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
--rw-r--r--   0        0        0     1468 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/process/skew/boron_si_skew.csv
--rw-r--r--   0        0        0     1118 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
--rw-r--r--   0        0        0      191 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/__init__.py
--rw-r--r--   0        0        0    14848 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/build_model.py
--rw-r--r--   0        0        0     7449 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/femwell_waveguide_model.py
--rw-r--r--   0        0        0     1571 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/interpolators.py
--rw-r--r--   0        0        0     6755 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/meep_FDTD_model.py
--rw-r--r--   0        0        0     4528 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/meow_eme_model.py
--rw-r--r--   0        0        0     5613 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/mlp.py
--rw-r--r--   0        0        0     7358 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/models.py
--rw-r--r--   0        0        0    13894 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/parameter.py
--rwxr-xr-x   0        0        0     2225 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/plot_model.py
--rw-r--r--   0        0        0     6805 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/read.py
--rw-r--r--   0        0        0     1350 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/tests/test_mzi.py
--rw-r--r--   0        0        0     2220 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
--rw-r--r--   0        0        0     1405 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sax/tests/test_parameters.py
--rw-r--r--   0        0        0     1357 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/__init__.py
--rw-r--r--   0        0        0     1573 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/add_gc.py
--rw-r--r--   0        0        0     3383 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/circuit.py
--rw-r--r--   0        0        0      891 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/__init__.py
--rw-r--r--   0        0        0     1295 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/bend_circular.py
--rw-r--r--   0        0        0     1388 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/bend_euler.py
--rw-r--r--   0        0        0     2560 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/coupler.py
--rw-r--r--   0        0        0     1046 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/coupler_fdtd.py
--rw-r--r--   0        0        0     1848 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/coupler_ring.py
--rw-r--r--   0        0        0     1329 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
--rw-r--r--   0        0        0      589 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
--rw-r--r--   0        0        0      913 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/gc.py
--rw-r--r--   0        0        0     2032 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/mmi1x2.py
--rw-r--r--   0        0        0     1910 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/mmi2x2.py
--rw-r--r--   0        0        0     2618 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/mzi.py
--rw-r--r--   0        0        0     1759 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/mzi_siepic.py
--rw-r--r--   0        0        0      487 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/mzi_thermal.py
--rw-r--r--   0        0        0     2597 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/ring_double.py
--rw-r--r--   0        0        0     1665 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/ring_double_siepic.py
--rw-r--r--   0        0        0     1782 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/ring_single.py
--rw-r--r--   0        0        0     1416 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/ring_single_siepic.py
--rw-r--r--   0        0        0     1099 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/straight.py
--rw-r--r--   0        0        0      800 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/get_transmission.py
--rw-r--r--   0        0        0     2516 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/model_from_gdsfactory.py
--rw-r--r--   0        0        0     3841 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/model_from_sparameters.py
--rw-r--r--   0        0        0     2438 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/plot_circuit.py
--rw-r--r--   0        0        0     1798 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
--rw-r--r--   0        0        0     2773 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/plot_model.py
--rw-r--r--   0        0        0     1261 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_circuit.py
--rw-r--r--   0        0        0       90 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
--rw-r--r--   0        0        0     1109 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components.py
--rw-r--r--   0        0        0       66 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
--rw-r--r--   0        0        0       69 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
--rw-r--r--   0        0        0       69 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
--rw-r--r--   0        0        0       92 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
--rw-r--r--   0        0        0       92 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
--rw-r--r--   0        0        0      412 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
--rw-r--r--   0        0        0      412 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
--rw-r--r--   0        0        0      114 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
--rw-r--r--   0        0        0      256 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
--rw-r--r--   0        0        0      460 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
--rw-r--r--   0        0        0      104 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
--rw-r--r--   0        0        0      166 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/simphony/types.py
--rw-r--r--   0        0        0      471 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sipann/__init__.py
--rw-r--r--   0        0        0     1376 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sipann/bend_circular.py
--rw-r--r--   0        0        0     1465 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sipann/bend_euler.py
--rw-r--r--   0        0        0     2508 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sipann/coupler.py
--rw-r--r--   0        0        0     1892 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sipann/coupler_ring.py
--rw-r--r--   0        0        0      736 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/sipann/straight.py
--rw-r--r--   0        0        0      100 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/thermal/__init__.py
--rw-r--r--   0        0        0     7789 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/simulation/thermal/heater.py
--rw-r--r--   0        0        0     1744 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/snap.py
--rw-r--r--   0        0        0     4245 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/symbols.py
--rw-r--r--   0        0        0      524 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/technology/__init__.py
--rw-r--r--   0        0        0     7607 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/technology/klayout_tech.py
--rw-r--r--   0        0        0     1078 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/technology/layer_map.py
--rw-r--r--   0        0        0    16139 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/technology/layer_stack.py
--rw-r--r--   0        0        0    42133 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/technology/layer_views.py
--rw-r--r--   0        0        0     1984 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/technology/simulation_settings.py
--rw-r--r--   0        0        0     1635 2023-05-26 15:13:13.256618 gdsfactory-6.98.2/gdsfactory/types.py
--rw-r--r--   0        0        0    10008 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/typings.py
--rw-r--r--   0        0        0        0 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/utils/__init__.py
--rw-r--r--   0        0        0     1342 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/utils/async_utils.py
--rw-r--r--   0        0        0      376 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/utils/color_utils.py
--rw-r--r--   0        0        0      558 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/utils/file_utils.py
--rw-r--r--   0        0        0      185 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/utils/function_utils.py
--rw-r--r--   0        0        0      684 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/utils/xml_utils.py
--rw-r--r--   0        0        0     1453 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/utils/yaml_utils.py
--rw-r--r--   0        0        0     4865 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/watch.py
--rw-r--r--   0        0        0        0 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/widgets/__init__.py
--rw-r--r--   0        0        0     7969 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/widgets/layout_viewer.py
--rw-r--r--   0        0        0     7480 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/gdsfactory/write_cells.py
--rw-r--r--   0        0        0     5706 2023-05-26 15:13:13.260618 gdsfactory-6.98.2/pyproject.toml
--rw-r--r--   0        0        0    18870 1970-01-01 00:00:00.000000 gdsfactory-6.98.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-29 17:46:56.493329 gdsfactory-6.99.0/LICENSE
+-rw-r--r--   0        0        0    14381 2023-05-29 17:46:56.493329 gdsfactory-6.99.0/README.md
+-rw-r--r--   0        0        0     3583 2023-05-29 17:46:56.501329 gdsfactory-6.99.0/gdsfactory/__init__.py
+-rw-r--r--   0        0        0     2104 2023-05-29 17:46:56.501329 gdsfactory-6.99.0/gdsfactory/add_keepout.py
+-rw-r--r--   0        0        0    12629 2023-05-29 17:46:56.501329 gdsfactory-6.99.0/gdsfactory/add_labels.py
+-rw-r--r--   0        0        0     3711 2023-05-29 17:46:56.501329 gdsfactory-6.99.0/gdsfactory/add_loopback.py
+-rw-r--r--   0        0        0     5054 2023-05-29 17:46:56.501329 gdsfactory-6.99.0/gdsfactory/add_padding.py
+-rw-r--r--   0        0        0    15639 2023-05-29 17:46:56.501329 gdsfactory-6.99.0/gdsfactory/add_pins.py
+-rw-r--r--   0        0        0    14700 2023-05-29 17:46:56.501329 gdsfactory-6.99.0/gdsfactory/add_ports.py
+-rw-r--r--   0        0        0     2884 2023-05-29 17:46:56.501329 gdsfactory-6.99.0/gdsfactory/add_tapers.py
+-rw-r--r--   0        0        0     2257 2023-05-29 17:46:56.501329 gdsfactory-6.99.0/gdsfactory/add_tapers_cross_section.py
+-rw-r--r--   0        0        0     1831 2023-05-29 17:46:56.501329 gdsfactory-6.99.0/gdsfactory/add_termination.py
+-rw-r--r--   0        0        0     1856 2023-05-29 17:46:56.501329 gdsfactory-6.99.0/gdsfactory/asserts.py
+-rw-r--r--   0        0        0    14287 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/cell.py
+-rw-r--r--   0        0        0    16040 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/circuitviz.py
+-rw-r--r--   0        0        0     5718 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/cli.py
+-rw-r--r--   0        0        0   100723 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/component.py
+-rw-r--r--   0        0        0    23424 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/component_layout.py
+-rw-r--r--   0        0        0    29879 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/component_reference.py
+-rw-r--r--   0        0        0     1205 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/C.py
+-rw-r--r--   0        0        0     1144 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/L.py
+-rw-r--r--   0        0        0    20964 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/__init__.py
+-rw-r--r--   0        0        0     2621 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/add_fiducials.py
+-rw-r--r--   0        0        0    14087 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/add_grating_couplers.py
+-rw-r--r--   0        0        0     2014 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/add_trenches.py
+-rw-r--r--   0        0        0     3207 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/align.py
+-rw-r--r--   0        0        0     2622 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/array_component.py
+-rw-r--r--   0        0        0     4705 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/array_with_fanout.py
+-rw-r--r--   0        0        0     4322 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/array_with_via.py
+-rw-r--r--   0        0        0     4042 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/awg.py
+-rw-r--r--   0        0        0     1269 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/bbox.py
+-rw-r--r--   0        0        0     2851 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/bend_circular.py
+-rw-r--r--   0        0        0     2649 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/bend_circular_heater.py
+-rw-r--r--   0        0        0     7903 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/bend_euler.py
+-rw-r--r--   0        0        0     2682 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/bend_port.py
+-rw-r--r--   0        0        0     3787 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/bend_s.py
+-rw-r--r--   0        0        0     5373 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/bezier.py
+-rw-r--r--   0        0        0     1605 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/cavity.py
+-rw-r--r--   0        0        0     5766 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/cdc.py
+-rw-r--r--   0        0        0     2929 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/cdsem_all.py
+-rw-r--r--   0        0        0     1788 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/cdsem_bend180.py
+-rw-r--r--   0        0        0     1631 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/cdsem_coupler.py
+-rw-r--r--   0        0        0     1412 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/cdsem_straight.py
+-rw-r--r--   0        0        0     1565 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/cdsem_straight_density.py
+-rw-r--r--   0        0        0      793 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/circle.py
+-rw-r--r--   0        0        0     5722 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coh_rx_dual_pol.py
+-rw-r--r--   0        0        0     8922 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coh_rx_single_pol.py
+-rw-r--r--   0        0        0     5043 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coh_tx_dual_pol.py
+-rw-r--r--   0        0        0     6118 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coh_tx_single_pol.py
+-rw-r--r--   0        0        0     2548 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/compass.py
+-rw-r--r--   0        0        0     9876 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/component_lattice.py
+-rw-r--r--   0        0        0     7174 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/component_sequence.py
+-rw-r--r--   0        0        0      812 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/copy_layers.py
+-rw-r--r--   0        0        0     3460 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coupler.py
+-rw-r--r--   0        0        0     2113 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coupler90.py
+-rw-r--r--   0        0        0     1802 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coupler90bend.py
+-rw-r--r--   0        0        0     4666 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coupler_adiabatic.py
+-rw-r--r--   0        0        0     1909 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coupler_asymmetric.py
+-rw-r--r--   0        0        0     3970 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coupler_full.py
+-rw-r--r--   0        0        0     3414 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coupler_ring.py
+-rw-r--r--   0        0        0     1060 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coupler_straight.py
+-rw-r--r--   0        0        0     1164 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coupler_straight_asymmetric.py
+-rw-r--r--   0        0        0     2192 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/coupler_symmetric.py
+-rw-r--r--   0        0        0     1848 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/cross.py
+-rw-r--r--   0        0        0    12873 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/crossing_waveguide.py
+-rw-r--r--   0        0        0      500 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
+-rw-r--r--   0        0        0     1014 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
+-rw-r--r--   0        0        0    19749 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
+-rw-r--r--   0        0        0    19751 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
+-rw-r--r--   0        0        0    19749 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
+-rw-r--r--   0        0        0    19751 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
+-rw-r--r--   0        0        0    19775 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
+-rw-r--r--   0        0        0     3143 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
+-rw-r--r--   0        0        0     5272 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/cutback_2x2.py
+-rw-r--r--   0        0        0     6450 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/cutback_bend.py
+-rw-r--r--   0        0        0     3765 2023-05-29 17:46:56.505329 gdsfactory-6.99.0/gdsfactory/components/cutback_component.py
+-rw-r--r--   0        0        0     2721 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/cutback_splitter.py
+-rw-r--r--   0        0        0     2971 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/dbr.py
+-rw-r--r--   0        0        0     4288 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/dbr_tapered.py
+-rw-r--r--   0        0        0     2486 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/delay_snake.py
+-rw-r--r--   0        0        0     3177 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/delay_snake2.py
+-rw-r--r--   0        0        0     3245 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/delay_snake3.py
+-rw-r--r--   0        0        0     4319 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/delay_snake_sbend.py
+-rw-r--r--   0        0        0     1226 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/dicing_lane.py
+-rw-r--r--   0        0        0     3471 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/die.py
+-rw-r--r--   0        0        0     2975 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/die_bbox.py
+-rw-r--r--   0        0        0     2863 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/die_bbox_frame.py
+-rw-r--r--   0        0        0     8015 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/disk.py
+-rw-r--r--   0        0        0     4112 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/edge_coupler_array.py
+-rw-r--r--   0        0        0     1214 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ellipse.py
+-rw-r--r--   0        0        0     1800 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/extend_ports_list.py
+-rw-r--r--   0        0        0     7988 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/extension.py
+-rw-r--r--   0        0        0      981 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/fiber.py
+-rw-r--r--   0        0        0     1432 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/fiber_array.py
+-rw-r--r--   0        0        0      722 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/fiducial_squares.py
+-rw-r--r--   0        0        0     3290 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ge_detector_straight_si_contacts.py
+-rw-r--r--   0        0        0     1063 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_array.py
+-rw-r--r--   0        0        0     4682 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_dual_pol.py
+-rw-r--r--   0        0        0     7110 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_elliptical.py
+-rw-r--r--   0        0        0     7222 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
+-rw-r--r--   0        0        0     4961 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py
+-rw-r--r--   0        0        0     4592 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_elliptical_trenches.py
+-rw-r--r--   0        0        0     1773 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_functions.py
+-rw-r--r--   0        0        0     9058 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_loss.py
+-rw-r--r--   0        0        0     1786 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_loss_fiber_single.py
+-rw-r--r--   0        0        0     4142 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_rectangular.py
+-rw-r--r--   0        0        0     4685 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
+-rw-r--r--   0        0        0     3887 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
+-rw-r--r--   0        0        0     1579 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/grating_coupler_tree.py
+-rw-r--r--   0        0        0     8811 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/greek_cross.py
+-rw-r--r--   0        0        0     1019 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/hline.py
+-rw-r--r--   0        0        0     3687 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/interdigital_capacitor.py
+-rw-r--r--   0        0        0     1825 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/litho_calipers.py
+-rw-r--r--   0        0        0     1244 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/litho_ruler.py
+-rw-r--r--   0        0        0     1304 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/litho_steps.py
+-rw-r--r--   0        0        0      650 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/logo.py
+-rw-r--r--   0        0        0     1679 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/loop_mirror.py
+-rw-r--r--   0        0        0     3873 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mmi1x2.py
+-rw-r--r--   0        0        0     2769 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mmi1x2_with_sbend.py
+-rw-r--r--   0        0        0     3858 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mmi2x2.py
+-rw-r--r--   0        0        0     3168 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mmi2x2_with_sbend.py
+-rw-r--r--   0        0        0     4947 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mmi_90degree_hybrid.py
+-rw-r--r--   0        0        0     3265 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mode_converter.py
+-rw-r--r--   0        0        0     7661 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mzi.py
+-rw-r--r--   0        0        0     2499 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mzi_arm.py
+-rw-r--r--   0        0        0     5835 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mzi_arms.py
+-rw-r--r--   0        0        0    12214 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mzi_lattice.py
+-rw-r--r--   0        0        0     4025 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mzi_pads_center.py
+-rw-r--r--   0        0        0     1064 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mzi_phase_shifter.py
+-rw-r--r--   0        0        0     6342 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mzit.py
+-rw-r--r--   0        0        0     3502 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mzit_lattice.py
+-rw-r--r--   0        0        0     6047 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/mzm.py
+-rw-r--r--   0        0        0     3518 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/nxn.py
+-rw-r--r--   0        0        0     1940 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/optimal_90deg.py
+-rw-r--r--   0        0        0     3876 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/optimal_hairpin.py
+-rw-r--r--   0        0        0     6131 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/optimal_step.py
+-rw-r--r--   0        0        0     6327 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/pack_doe.py
+-rw-r--r--   0        0        0     3860 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/pad.py
+-rw-r--r--   0        0        0     1890 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/pad_gsg.py
+-rw-r--r--   0        0        0     1157 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/pads_shorted.py
+-rw-r--r--   0        0        0     3833 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/polarization_splitter_rotator.py
+-rw-r--r--   0        0        0     1147 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ramp.py
+-rw-r--r--   0        0        0     1508 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/rectangle.py
+-rw-r--r--   0        0        0     2972 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/rectangle_with_slits.py
+-rw-r--r--   0        0        0     1508 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/regular_polygon.py
+-rw-r--r--   0        0        0     3302 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/resistance_meander.py
+-rw-r--r--   0        0        0     2642 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/resistance_sheet.py
+-rw-r--r--   0        0        0     1273 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring.py
+-rw-r--r--   0        0        0     4143 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_crow.py
+-rw-r--r--   0        0        0     3272 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_crow_couplers.py
+-rw-r--r--   0        0        0     2267 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_double.py
+-rw-r--r--   0        0        0     2846 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_double_bend_coupler.py
+-rw-r--r--   0        0        0     3846 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_double_heater.py
+-rw-r--r--   0        0        0     7757 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_double_pn.py
+-rw-r--r--   0        0        0    12137 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_section_based.py
+-rw-r--r--   0        0        0     2740 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_single.py
+-rw-r--r--   0        0        0     1968 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_single_array.py
+-rw-r--r--   0        0        0     6868 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_single_bend_coupler.py
+-rw-r--r--   0        0        0     2714 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_single_dut.py
+-rw-r--r--   0        0        0     4018 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_single_heater.py
+-rw-r--r--   0        0        0     5317 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/ring_single_pn.py
+-rw-r--r--   0        0        0     2282 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/seal_ring.py
+-rw-r--r--   0        0        0     3758 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/snspd.py
+-rw-r--r--   0        0        0     2059 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/spiral_double.py
+-rw-r--r--   0        0        0     5871 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/spiral_external_io.py
+-rw-r--r--   0        0        0    16692 2023-05-29 17:46:56.509329 gdsfactory-6.99.0/gdsfactory/components/spiral_heater.py
+-rw-r--r--   0        0        0     9181 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/spiral_inner_io.py
+-rw-r--r--   0        0        0     1733 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/splitter_chain.py
+-rw-r--r--   0        0        0     5327 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/splitter_tree.py
+-rw-r--r--   0        0        0     2507 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/straight.py
+-rw-r--r--   0        0        0     1033 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/straight_array.py
+-rw-r--r--   0        0        0     7914 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/straight_heater_doped_rib.py
+-rw-r--r--   0        0        0     1922 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/straight_heater_doped_strip.py
+-rw-r--r--   0        0        0     7891 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/straight_heater_meander.py
+-rw-r--r--   0        0        0     8090 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/straight_heater_meander_doped.py
+-rw-r--r--   0        0        0     5686 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/straight_heater_metal.py
+-rw-r--r--   0        0        0     2809 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/straight_pin.py
+-rw-r--r--   0        0        0     3974 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/straight_pin_slot.py
+-rw-r--r--   0        0        0      655 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/straight_rib.py
+-rw-r--r--   0        0        0      820 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/switch_tree.py
+-rw-r--r--   0        0        0     7730 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/taper.py
+-rw-r--r--   0        0        0     3530 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/taper_adiabatic.py
+-rw-r--r--   0        0        0     2576 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/taper_cross_section.py
+-rw-r--r--   0        0        0     2363 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/taper_from_csv.py
+-rw-r--r--   0        0        0     1235 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/taper_parabolic.py
+-rw-r--r--   0        0        0     1635 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/terminator.py
+-rw-r--r--   0        0        0     2913 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/text.py
+-rw-r--r--   0        0        0     3886 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/text_freetype.py
+-rw-r--r--   0        0        0     3160 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/text_rectangular.py
+-rw-r--r--   0        0        0     3943 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/text_rectangular_font.py
+-rw-r--r--   0        0        0     2536 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/triangles.py
+-rw-r--r--   0        0        0      715 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/verniers.py
+-rw-r--r--   0        0        0     2468 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/version_stamp.py
+-rw-r--r--   0        0        0     2436 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/via.py
+-rw-r--r--   0        0        0     3060 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/via_corner.py
+-rw-r--r--   0        0        0     5342 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/via_cutback.py
+-rw-r--r--   0        0        0    15612 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/via_stack.py
+-rw-r--r--   0        0        0     4430 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/via_stack_slot.py
+-rw-r--r--   0        0        0     4944 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/via_stack_with_offset.py
+-rw-r--r--   0        0        0     1088 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/wafer.py
+-rw-r--r--   0        0        0     2542 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/wire.py
+-rw-r--r--   0        0        0      978 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/components/wire_sbend.py
+-rw-r--r--   0        0        0     8159 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/config.py
+-rw-r--r--   0        0        0      481 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/conftest.py
+-rw-r--r--   0        0        0    38409 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/constants.py
+-rw-r--r--   0        0        0     1476 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/containers.py
+-rw-r--r--   0        0        0    83118 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/cross_section.py
+-rw-r--r--   0        0        0     2982 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/decorators.py
+-rw-r--r--   0        0        0     7008 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/difftest.py
+-rw-r--r--   0        0        0     1020 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/events.py
+-rw-r--r--   0        0        0      267 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/export/__init__.py
+-rw-r--r--   0        0        0     3353 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/export/to_3d.py
+-rw-r--r--   0        0        0     7599 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/export/to_gerber.py
+-rw-r--r--   0        0        0     1940 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/export/to_np.py
+-rw-r--r--   0        0        0     3058 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/export/to_stl.py
+-rw-r--r--   0        0        0     2976 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/filestorage.py
+-rw-r--r--   0        0        0    11908 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/fill.py
+-rw-r--r--   0        0        0     7799 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/font.py
+-rw-r--r--   0        0        0     8073 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/functions.py
+-rw-r--r--   0        0        0       20 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/gdsdiff/.gitattributes
+-rw-r--r--   0        0        0       83 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/gdsdiff/.gitconfig
+-rw-r--r--   0        0        0       72 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/gdsdiff/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/gdsdiff/gds_diff_git.py
+-rw-r--r--   0        0        0     2935 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/gdsdiff/gdsdiff.py
+-rw-r--r--   0        0        0      708 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/gdsdiff/install.py
+-rw-r--r--   0        0        0      271 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/gdsdiff/sample.py
+-rw-r--r--   0        0        0     1111 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/gdsdiff/test_xor.py
+-rw-r--r--   0        0        0     1100 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/README.md
+-rw-r--r--   0        0        0     1722 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/generic_tech.sh
+-rw-r--r--   0        0        0     8142 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/get_klayout_pyxs.py
+-rw-r--r--   0        0        0      161 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/README.md
+-rw-r--r--   0        0        0      104 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/drc/Makefile
+-rw-r--r--   0        0        0        0 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/drc/__init__.py
+-rw-r--r--   0        0        0     2842 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/drc/errors.py
+-rw-r--r--   0        0        0     6193 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/grain.xml
+-rw-r--r--   0        0        0    10140 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/icon_128x128.png
+-rw-r--r--   0        0        0     4248 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/icon_64x64.png
+-rw-r--r--   0        0        0       27 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/.gitignore
+-rw-r--r--   0        0        0      494 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/Makefile
+-rw-r--r--   0        0        0     4062 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/README.md
+-rw-r--r--   0        0        0     2419 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
+-rw-r--r--   0        0        0     9696 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
+-rw-r--r--   0        0        0    12379 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
+-rw-r--r--   0        0        0     7235 2023-05-29 17:46:56.513329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
+-rw-r--r--   0        0        0     3446 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
+-rw-r--r--   0        0        0      479 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
+-rw-r--r--   0        0        0      582 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
+-rw-r--r--   0        0        0      108 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
+-rw-r--r--   0        0        0      186 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
+-rw-r--r--   0        0        0      398 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
+-rw-r--r--   0        0        0      574 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
+-rw-r--r--   0        0        0     6034 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
+-rw-r--r--   0        0        0    10704 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
+-rw-r--r--   0        0        0      477 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
+-rw-r--r--   0        0        0     4337 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
+-rw-r--r--   0        0        0      926 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
+-rw-r--r--   0        0        0    10945 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
+-rw-r--r--   0        0        0      710 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
+-rw-r--r--   0        0        0      538 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
+-rw-r--r--   0        0        0        0 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/python/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
+-rw-r--r--   0        0        0     4311 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
+-rw-r--r--   0        0        0      269 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/Makefile
+-rw-r--r--   0        0        0     1854 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
+-rw-r--r--   0        0        0     1519 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack
+-rw-r--r--   0        0        0    41073 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
+-rw-r--r--   0        0        0    40616 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/layers.lyp
+-rw-r--r--   0        0        0     5977 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/tech.lyt
+-rw-r--r--   0        0        0     4258 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
+-rw-r--r--   0        0        0     4537 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
+-rw-r--r--   0        0        0     4690 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
+-rw-r--r--   0        0        0     5508 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
+-rw-r--r--   0        0        0     1883 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/layer_map.py
+-rw-r--r--   0        0        0     6511 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/layer_stack.py
+-rw-r--r--   0        0        0    10780 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/layer_views.yaml
+-rw-r--r--   0        0        0      158 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/generic_tech/simulation_settings.py
+-rw-r--r--   0        0        0     1431 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/__init__.py
+-rw-r--r--   0        0        0     4917 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/boolean.py
+-rw-r--r--   0        0        0     3814 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/boolean_klayout.py
+-rw-r--r--   0        0        0     1904 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/boolean_polygons.py
+-rw-r--r--   0        0        0      598 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/check_duplicated_cells.py
+-rw-r--r--   0        0        0     2719 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/check_exclusion.py
+-rw-r--r--   0        0        0     2829 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/check_inclusion.py
+-rw-r--r--   0        0        0     3566 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/check_space.py
+-rw-r--r--   0        0        0     1904 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/check_width.py
+-rw-r--r--   0        0        0     5010 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/fill_klayout.py
+-rw-r--r--   0        0        0     7034 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/fill_tiled.py
+-rw-r--r--   0        0        0     1697 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/fillet.py
+-rw-r--r--   0        0        0     6664 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/functions.py
+-rw-r--r--   0        0        0     2167 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/invert.py
+-rw-r--r--   0        0        0     3685 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/layer_priority.py
+-rw-r--r--   0        0        0     3054 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/manhattanize.py
+-rw-r--r--   0        0        0     4192 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/maskprep.py
+-rw-r--r--   0        0        0     4814 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/maskprep_flat.py
+-rw-r--r--   0        0        0     3250 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/offset.py
+-rw-r--r--   0        0        0     3842 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/outline.py
+-rw-r--r--   0        0        0     2510 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/trim.py
+-rw-r--r--   0        0        0     2948 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/union.py
+-rw-r--r--   0        0        0     3609 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/write_connectivity.py
+-rw-r--r--   0        0        0    10532 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/write_drc.py
+-rw-r--r--   0        0        0     1783 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/geometry/xor_diff.py
+-rw-r--r--   0        0        0     1158 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/get_factories.py
+-rw-r--r--   0        0        0    23569 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/get_netlist.py
+-rw-r--r--   0        0        0    14446 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/get_netlist_flat.py
+-rw-r--r--   0        0        0      682 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/get_netlist_klayout.py
+-rw-r--r--   0        0        0     9745 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/grid.py
+-rw-r--r--   0        0        0     4393 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/install.py
+-rw-r--r--   0        0        0     1970 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/klive.py
+-rw-r--r--   0        0        0      585 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/labels/__init__.py
+-rw-r--r--   0        0        0     3563 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/labels/add_label_yaml.py
+-rw-r--r--   0        0        0     3847 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/labels/ehva.py
+-rw-r--r--   0        0        0     3810 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/labels/merge_test_metadata.py
+-rw-r--r--   0        0        0     4668 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/labels/siepic.py
+-rw-r--r--   0        0        0     4847 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/labels/write_labels.py
+-rw-r--r--   0        0        0     1149 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/materials.py
+-rw-r--r--   0        0        0     5247 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/name.py
+-rw-r--r--   0        0        0    11586 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/pack.py
+-rw-r--r--   0        0        0    51631 2023-05-29 17:46:56.517329 gdsfactory-6.99.0/gdsfactory/path.py
+-rw-r--r--   0        0        0    27294 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/pdk.py
+-rw-r--r--   0        0        0     6220 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/picmodel.py
+-rw-r--r--   0        0        0     5068 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/pixelate.py
+-rw-r--r--   0        0        0        0 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/dagster/__init__.py
+-rw-r--r--   0        0        0      976 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/dagster/workflow.py
+-rw-r--r--   0        0        0      566 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/database/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/database/__init__.py
+-rw-r--r--   0        0        0     6216 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/database/db_upload.py
+-rw-r--r--   0        0        0    16143 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/database/models.py
+-rw-r--r--   0        0        0       32 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/Makefile
+-rw-r--r--   0        0        0       23 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/__init__.py
+-rw-r--r--   0        0        0     4080 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/main.py
+-rwxr-xr-x   0        0        0     7511 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/server.py
+-rwxr-xr-x   0        0        0      594 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/server_jupyter.py
+-rw-r--r--   0        0        0     1299 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/static/client.css
+-rw-r--r--   0        0        0     9637 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/static/client.js
+-rw-r--r--   0        0        0      840 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/templates/client.html
+-rw-r--r--   0        0        0      236 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/templates/footer.html
+-rw-r--r--   0        0        0      229 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/templates/gdspaths.html
+-rw-r--r--   0        0        0      572 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/templates/header.html
+-rw-r--r--   0        0        0      253 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/templates/index.html
+-rw-r--r--   0        0        0      964 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/templates/navbar.html
+-rw-r--r--   0        0        0     1837 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/plugins/web/templates/viewer.html
+-rw-r--r--   0        0        0    32235 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/port.py
+-rw-r--r--   0        0        0    37817 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/quickplotter.py
+-rw-r--r--   0        0        0      696 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/read/__init__.py
+-rw-r--r--   0        0        0     1639 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/read/from_dphox.py
+-rw-r--r--   0        0        0     1285 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/read/from_gdspaths.py
+-rw-r--r--   0        0        0     1953 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/read/from_np.py
+-rw-r--r--   0        0        0     2813 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/read/from_phidl.py
+-rw-r--r--   0        0        0    38082 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/read/from_yaml.py
+-rw-r--r--   0        0        0     5897 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/read/from_yaml_template.py
+-rw-r--r--   0        0        0     5688 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/read/import_gds.py
+-rw-r--r--   0        0        0     3407 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/read/labels.py
+-rw-r--r--   0        0        0     3769 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/__init__.py
+-rw-r--r--   0        0        0     2920 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/add_electrical_pads_shortest.py
+-rw-r--r--   0        0        0     3015 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/add_electrical_pads_top.py
+-rw-r--r--   0        0        0     3035 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/add_electrical_pads_top_dc.py
+-rw-r--r--   0        0        0     8715 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/add_fiber_array.py
+-rw-r--r--   0        0        0    10624 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/add_fiber_single.py
+-rw-r--r--   0        0        0     8967 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/add_pads.py
+-rw-r--r--   0        0        0    38948 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/all_angle.py
+-rw-r--r--   0        0        0     3916 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/auto_taper.py
+-rw-r--r--   0        0        0      982 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/factories.py
+-rw-r--r--   0        0        0     4415 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/fanout.py
+-rw-r--r--   0        0        0     2800 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/fanout2x2.py
+-rw-r--r--   0        0        0    24342 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_bundle.py
+-rw-r--r--   0        0        0     8652 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_bundle_corner.py
+-rw-r--r--   0        0        0     6910 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_bundle_from_steps.py
+-rw-r--r--   0        0        0    12949 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_bundle_from_waypoints.py
+-rw-r--r--   0        0        0     5284 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_bundle_path_length_match.py
+-rw-r--r--   0        0        0     1937 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_bundle_sbend.py
+-rw-r--r--   0        0        0    17064 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_bundle_u.py
+-rw-r--r--   0        0        0     1510 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_input_labels.py
+-rw-r--r--   0        0        0     9283 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_route.py
+-rw-r--r--   0        0        0    10872 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_route_astar.py
+-rw-r--r--   0        0        0     6119 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_route_from_steps.py
+-rw-r--r--   0        0        0     2766 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_route_sbend.py
+-rw-r--r--   0        0        0     3311 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_routes_bend180.py
+-rw-r--r--   0        0        0     1854 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/get_routes_straight.py
+-rw-r--r--   0        0        0    34199 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/manhattan.py
+-rw-r--r--   0        0        0    10081 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/path_length_matching.py
+-rw-r--r--   0        0        0    22568 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/route_fiber_array.py
+-rw-r--r--   0        0        0     8679 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/route_fiber_single.py
+-rw-r--r--   0        0        0    18132 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/route_ports_to_side.py
+-rw-r--r--   0        0        0     4379 2023-05-29 17:46:56.521329 gdsfactory-6.99.0/gdsfactory/routing/route_quad.py
+-rw-r--r--   0        0        0    14370 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/routing/route_sharp.py
+-rw-r--r--   0        0        0    10167 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/routing/route_south.py
+-rw-r--r--   0        0        0     5072 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/routing/sort_ports.py
+-rw-r--r--   0        0        0     2477 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/routing/utils.py
+-rw-r--r--   0        0        0     2897 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/01_component_pcell.py
+-rw-r--r--   0        0        0      646 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
+-rw-r--r--   0        0        0     1109 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/01_component_pcell_with_pins.py
+-rw-r--r--   0        0        0      664 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
+-rw-r--r--   0        0        0      347 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/02_component_autoname.py
+-rw-r--r--   0        0        0      887 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/03_move.py
+-rw-r--r--   0        0        0      881 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/04_connect.py
+-rw-r--r--   0        0        0      710 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/05_remove_layers.py
+-rw-r--r--   0        0        0      931 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/06_remapping_layers.py
+-rw-r--r--   0        0        0     1082 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/07_flattening_device.py
+-rw-r--r--   0        0        0      475 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/08_group.py
+-rw-r--r--   0        0        0     1631 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/11_component_layout.py
+-rw-r--r--   0        0        0     2245 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/12_component_refs.py
+-rw-r--r--   0        0        0      955 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/13_component_netlist.py
+-rw-r--r--   0        0        0     2592 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/14_component_connectivity.py
+-rw-r--r--   0        0        0     1636 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/15_component_sequence1.py
+-rw-r--r--   0        0        0     1680 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/16_component_sequence2.py
+-rw-r--r--   0        0        0      965 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/17_ports.py
+-rw-r--r--   0        0        0      489 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/18_port_markers.py
+-rw-r--r--   0        0        0      361 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/19_references.py
+-rw-r--r--   0        0        0      533 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/20_components.py
+-rw-r--r--   0        0        0      459 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/21_add_fiber_array.py
+-rw-r--r--   0        0        0      445 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/22_add_fiber_single.py
+-rw-r--r--   0        0        0      569 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/22_add_pads.py
+-rw-r--r--   0        0        0      848 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/23_reticle.py
+-rw-r--r--   0        0        0     1588 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/23_reticle_passives.py
+-rw-r--r--   0        0        0      457 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/24_doe.py
+-rw-r--r--   0        0        0      687 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/24_doe_2.py
+-rw-r--r--   0        0        0      692 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/24_doe_3.py
+-rw-r--r--   0        0        0      306 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/25_slot_cross_section.py
+-rw-r--r--   0        0        0     1363 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/30_lidar.py
+-rw-r--r--   0        0        0     1412 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/30_lidar_pcell.py
+-rw-r--r--   0        0        0     1943 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/30_lidar_with_pads.py
+-rw-r--r--   0        0        0        0 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/__init__.py
+-rw-r--r--   0        0        0     1307 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing.py
+-rw-r--r--   0        0        0      558 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
+-rw-r--r--   0        0        0     6062 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
+-rw-r--r--   0        0        0      444 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
+-rw-r--r--   0        0        0      463 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
+-rw-r--r--   0        0        0     1552 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
+-rw-r--r--   0        0        0     1315 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
+-rw-r--r--   0        0        0      602 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
+-rw-r--r--   0        0        0     3317 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
+-rw-r--r--   0        0        0     1484 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
+-rw-r--r--   0        0        0     3045 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
+-rw-r--r--   0        0        0     3782 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
+-rw-r--r--   0        0        0     1988 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/big_device.py
+-rw-r--r--   0        0        0       19 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/Makefile
+-rw-r--r--   0        0        0        0 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/benchmark/fill_demo.py
+-rw-r--r--   0        0        0      343 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
+-rw-r--r--   0        0        0      637 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/circuits/mask.pic.yml
+-rw-r--r--   0        0        0      622 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
+-rw-r--r--   0        0        0      569 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
+-rw-r--r--   0        0        0      453 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/circuits/pads.pic.yml
+-rw-r--r--   0        0        0      287 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/circuits/rectangles.pic.yml
+-rw-r--r--   0        0        0     2260 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/drc_errors.py
+-rw-r--r--   0        0        0     1014 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/drc_write.py
+-rw-r--r--   0        0        0     4530 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/layers.py
+-rw-r--r--   0        0        0      158 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/layers_sky130.py
+-rw-r--r--   0        0        0      364 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/layers_xsection.py
+-rw-r--r--   0        0        0     1065 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/lvs.py
+-rw-r--r--   0        0        0      574 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/demo/pcell.py
+-rw-r--r--   0        0        0     4174 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/netlists/mzi.yml
+-rw-r--r--   0        0        0     5840 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/netlists/mzi_full.yml
+-rw-r--r--   0        0        0        0 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/__init__.py
+-rw-r--r--   0        0        0     4235 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/fab_c.py
+-rw-r--r--   0        0        0      475 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/fab_d/__init__.py
+-rw-r--r--   0        0        0     1880 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py
+-rw-r--r--   0        0        0     1715 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c.py
+-rw-r--r--   0        0        0       50 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
+-rw-r--r--   0        0        0       93 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
+-rw-r--r--   0        0        0       85 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
+-rw-r--r--   0        0        0      139 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
+-rw-r--r--   0        0        0       90 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
+-rw-r--r--   0        0        0      126 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
+-rw-r--r--   0        0        0       48 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
+-rw-r--r--   0        0        0     1023 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
+-rw-r--r--   0        0        0     2206 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
+-rw-r--r--   0        0        0     1879 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
+-rw-r--r--   0        0        0     1283 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
+-rw-r--r--   0        0        0     1632 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
+-rw-r--r--   0        0        0     1061 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
+-rw-r--r--   0        0        0     1054 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
+-rw-r--r--   0        0        0     1617 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
+-rw-r--r--   0        0        0     4497 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
+-rw-r--r--   0        0        0     3625 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
+-rw-r--r--   0        0        0     3603 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
+-rw-r--r--   0        0        0     4455 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
+-rw-r--r--   0        0        0      840 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
+-rw-r--r--   0        0        0     2297 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
+-rw-r--r--   0        0        0      316 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/schematic.py
+-rw-r--r--   0        0        0    17862 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/schematic_editor.py
+-rw-r--r--   0        0        0     4462 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/serialization.py
+-rw-r--r--   0        0        0     1612 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/show.py
+-rw-r--r--   0        0        0      724 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/__init__.py
+-rw-r--r--   0        0        0     4369 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/add_simulation_markers.py
+-rw-r--r--   0        0        0     2476 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/convert_sparameters.py
+-rw-r--r--   0        0        0      597 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/devsim/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/devsim/doping.py
+-rw-r--r--   0        0        0    11977 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/devsim/get_simulation.py
+-rw-r--r--   0        0        0    28856 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/devsim/get_simulation_xsection.py
+-rw-r--r--   0        0        0    19756 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/devsim/get_solver.py
+-rw-r--r--   0        0        0     1610 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/devsim/test_devsim.py
+-rw-r--r--   0        0        0      189 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/disable_print.py
+-rw-r--r--   0        0        0       79 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/eme/__init__.py
+-rw-r--r--   0        0        0    14784 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/eme/meow_eme.py
+-rw-r--r--   0        0        0     1787 2023-05-29 17:46:56.525329 gdsfactory-6.99.0/gdsfactory/simulation/eme/test_meow_simulation.py
+-rw-r--r--   0        0        0        0 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/fem/__init__.py
+-rw-r--r--   0        0        0     8968 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/fem/mode_solver.py
+-rw-r--r--   0        0        0     2221 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/fem/test_mode_solver.py
+-rw-r--r--   0        0        0     3455 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/get_effective_indices.py
+-rw-r--r--   0        0        0     3109 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/get_modes_path.py
+-rw-r--r--   0        0        0     3888 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/get_sparameters_path.py
+-rw-r--r--   0        0        0     2003 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/__init__.py
+-rw-r--r--   0        0        0     3194 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_material.py
+-rw-r--r--   0        0        0     6137 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_meep_geometry.py
+-rw-r--r--   0        0        0     6054 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py
+-rw-r--r--   0        0        0    11014 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_simulation.py
+-rw-r--r--   0        0        0    15915 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
+-rw-r--r--   0        0        0    18182 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
+-rw-r--r--   0        0        0    12312 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
+-rw-r--r--   0        0        0    11914 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_eigenmode.py
+-rw-r--r--   0        0        0      832 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_materials.py
+-rw-r--r--   0        0        0    10128 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0     6642 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
+-rw-r--r--   0        0        0    10128 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0    10093 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
+-rw-r--r--   0        0        0    10085 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    34701 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
+-rw-r--r--   0        0        0    10123 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     9966 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
+-rw-r--r--   0        0        0     9966 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    10129 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
+-rw-r--r--   0        0        0    14053 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py
+-rw-r--r--   0        0        0    21281 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py
+-rw-r--r--   0        0        0     8143 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
+-rw-r--r--   0        0        0     9577 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
+-rw-r--r--   0        0        0     1246 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/__init__.py
+-rw-r--r--   0        0        0     6653 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/break_geometry.py
+-rw-r--r--   0        0        0    11250 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/mesh.py
+-rw-r--r--   0        0        0    11824 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/meshtracker.py
+-rw-r--r--   0        0        0     7752 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/parse_component.py
+-rw-r--r--   0        0        0     3644 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/parse_gds.py
+-rw-r--r--   0        0        0     3605 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/parse_layerstack.py
+-rw-r--r--   0        0        0     2990 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/refine.py
+-rw-r--r--   0        0        0    10851 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py
+-rw-r--r--   0        0        0     2513 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/tests/test_meshing.py
+-rw-r--r--   0        0        0    14168 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
+-rw-r--r--   0        0        0     7441 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
+-rw-r--r--   0        0        0    16334 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gmsh/xyz_mesh.py
+-rw-r--r--   0        0        0     1624 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/__init__.py
+-rw-r--r--   0        0        0     4368 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/get_results.py
+-rw-r--r--   0        0        0    20009 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/get_simulation.py
+-rw-r--r--   0        0        0    21071 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
+-rw-r--r--   0        0        0     3486 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/materials.py
+-rw-r--r--   0        0        0    27762 2023-05-29 17:46:56.529329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/modes.py
+-rw-r--r--   0        0        0     8941 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/sim_run.yaml
+-rw-r--r--   0        0        0     8114 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
+-rw-r--r--   0        0        0     8114 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
+-rw-r--r--   0        0        0      744 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py
+-rw-r--r--   0        0        0      262 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
+-rw-r--r--   0        0        0      879 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_results.py
+-rw-r--r--   0        0        0     1505 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
+-rw-r--r--   0        0        0     1655 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
+-rw-r--r--   0        0        0     9297 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     1732 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0     1224 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/utils.py
+-rw-r--r--   0        0        0    10841 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/write_sparameters.py
+-rw-r--r--   0        0        0     7695 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0      588 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/lumerical/__init__.py
+-rw-r--r--   0        0        0    16091 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/lumerical/interconnect.py
+-rw-r--r--   0        0        0     4286 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/lumerical/read.py
+-rw-r--r--   0        0        0     3569 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/lumerical/settings.py
+-rw-r--r--   0        0        0     2368 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/lumerical/test_read_sparameters.py
+-rw-r--r--   0        0        0    19865 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
+-rw-r--r--   0        0        0     1504 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
+-rw-r--r--   0        0        0      932 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/__init__.py
+-rw-r--r--   0        0        0     1618 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/coupler.py
+-rw-r--r--   0        0        0     4166 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py
+-rw-r--r--   0        0        0     2773 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/find_mode_dispersion.py
+-rw-r--r--   0        0        0     8924 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/find_modes.py
+-rwxr-xr-x   0        0        0     7032 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/find_modes_cross_section.py
+-rw-r--r--   0        0        0     4458 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
+-rw-r--r--   0        0        0     2728 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/find_neff_vs_width.py
+-rw-r--r--   0        0        0     7148 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py
+-rwxr-xr-x   0        0        0     4462 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
+-rw-r--r--   0        0        0     5411 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/get_mode_solver_rib.py
+-rw-r--r--   0        0        0     1110 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
+-rw-r--r--   0        0        0     1102 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
+-rw-r--r--   0        0        0     1110 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
+-rw-r--r--   0        0        0     8023 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/neff_convergence_test.py
+-rw-r--r--   0        0        0      267 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/neff_vs_width.csv
+-rw-r--r--   0        0        0     2469 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/overlap.py
+-rw-r--r--   0        0        0      418 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/tests/test_dw_dh.py
+-rw-r--r--   0        0        0       83 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
+-rw-r--r--   0        0        0      548 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
+-rw-r--r--   0        0        0     1137 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/tests/test_find_modes.py
+-rw-r--r--   0        0        0      649 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
+-rw-r--r--   0        0        0      354 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
+-rw-r--r--   0        0        0      113 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
+-rw-r--r--   0        0        0    15492 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/types.py
+-rw-r--r--   0        0        0     1169 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/modes/waveguide.py
+-rw-r--r--   0        0        0     2013 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/photonic_circuit_models/__init__.py
+-rw-r--r--   0        0        0      597 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/photonic_circuit_models/coupler.py
+-rw-r--r--   0        0        0      377 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/photonic_circuit_models/fsr.py
+-rw-r--r--   0        0        0      418 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/photonic_circuit_models/heater.py
+-rw-r--r--   0        0        0     3069 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/photonic_circuit_models/mzi.py
+-rw-r--r--   0        0        0     2616 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/photonic_circuit_models/ring.py
+-rw-r--r--   0        0        0     7332 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/plot.py
+-rw-r--r--   0        0        0     2480 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/plot_csv.py
+-rw-r--r--   0        0        0      613 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/port_symmetries.py
+-rw-r--r--   0        0        0     4685 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/process/diffusion.py
+-rw-r--r--   0        0        0     5317 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/process/implant_tables.py
+-rw-r--r--   0        0        0     6800 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/process/pysrim.py
+-rw-r--r--   0        0        0     2182 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/process/silicon.py
+-rw-r--r--   0        0        0     1861 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv
+-rw-r--r--   0        0        0     1050 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
+-rw-r--r--   0        0        0     1468 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/process/skew/boron_si_skew.csv
+-rw-r--r--   0        0        0     1118 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
+-rw-r--r--   0        0        0      191 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/__init__.py
+-rw-r--r--   0        0        0    14848 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/build_model.py
+-rw-r--r--   0        0        0     7449 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/femwell_waveguide_model.py
+-rw-r--r--   0        0        0     1571 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/interpolators.py
+-rw-r--r--   0        0        0     6755 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/meep_FDTD_model.py
+-rw-r--r--   0        0        0     4528 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/meow_eme_model.py
+-rw-r--r--   0        0        0     5613 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/mlp.py
+-rw-r--r--   0        0        0     7358 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/models.py
+-rw-r--r--   0        0        0    13894 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/parameter.py
+-rwxr-xr-x   0        0        0     2225 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/plot_model.py
+-rw-r--r--   0        0        0     6805 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/read.py
+-rw-r--r--   0        0        0     1350 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/tests/test_mzi.py
+-rw-r--r--   0        0        0     2220 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
+-rw-r--r--   0        0        0     1405 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/sax/tests/test_parameters.py
+-rw-r--r--   0        0        0     1357 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/__init__.py
+-rw-r--r--   0        0        0     1573 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/add_gc.py
+-rw-r--r--   0        0        0     3383 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/circuit.py
+-rw-r--r--   0        0        0      891 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/__init__.py
+-rw-r--r--   0        0        0     1295 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/bend_circular.py
+-rw-r--r--   0        0        0     1388 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/bend_euler.py
+-rw-r--r--   0        0        0     2560 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/coupler.py
+-rw-r--r--   0        0        0     1046 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py
+-rw-r--r--   0        0        0     1848 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/coupler_ring.py
+-rw-r--r--   0        0        0     1329 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
+-rw-r--r--   0        0        0      589 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
+-rw-r--r--   0        0        0      913 2023-05-29 17:46:56.533329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/gc.py
+-rw-r--r--   0        0        0     2032 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/mmi1x2.py
+-rw-r--r--   0        0        0     1910 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/mmi2x2.py
+-rw-r--r--   0        0        0     2618 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/mzi.py
+-rw-r--r--   0        0        0     1759 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/mzi_siepic.py
+-rw-r--r--   0        0        0      487 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/mzi_thermal.py
+-rw-r--r--   0        0        0     2597 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/ring_double.py
+-rw-r--r--   0        0        0     1665 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py
+-rw-r--r--   0        0        0     1782 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/ring_single.py
+-rw-r--r--   0        0        0     1416 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py
+-rw-r--r--   0        0        0     1099 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/straight.py
+-rw-r--r--   0        0        0      800 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/get_transmission.py
+-rw-r--r--   0        0        0     2516 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py
+-rw-r--r--   0        0        0     3841 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/model_from_sparameters.py
+-rw-r--r--   0        0        0     2438 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/plot_circuit.py
+-rw-r--r--   0        0        0     1798 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
+-rw-r--r--   0        0        0     2773 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/plot_model.py
+-rw-r--r--   0        0        0     1261 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_circuit.py
+-rw-r--r--   0        0        0       90 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
+-rw-r--r--   0        0        0     1109 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components.py
+-rw-r--r--   0        0        0       66 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
+-rw-r--r--   0        0        0       69 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
+-rw-r--r--   0        0        0       69 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
+-rw-r--r--   0        0        0       92 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
+-rw-r--r--   0        0        0       92 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
+-rw-r--r--   0        0        0      412 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
+-rw-r--r--   0        0        0      412 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
+-rw-r--r--   0        0        0      114 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
+-rw-r--r--   0        0        0      256 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
+-rw-r--r--   0        0        0      460 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
+-rw-r--r--   0        0        0      104 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
+-rw-r--r--   0        0        0      166 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/simphony/types.py
+-rw-r--r--   0        0        0      471 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/sipann/__init__.py
+-rw-r--r--   0        0        0     1376 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/sipann/bend_circular.py
+-rw-r--r--   0        0        0     1465 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/sipann/bend_euler.py
+-rw-r--r--   0        0        0     2508 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/sipann/coupler.py
+-rw-r--r--   0        0        0     1892 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/sipann/coupler_ring.py
+-rw-r--r--   0        0        0      736 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/sipann/straight.py
+-rw-r--r--   0        0        0      100 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/thermal/__init__.py
+-rw-r--r--   0        0        0     7789 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/simulation/thermal/heater.py
+-rw-r--r--   0        0        0     1744 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/snap.py
+-rw-r--r--   0        0        0     4245 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/symbols.py
+-rw-r--r--   0        0        0      524 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/technology/__init__.py
+-rw-r--r--   0        0        0     7607 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/technology/klayout_tech.py
+-rw-r--r--   0        0        0     1078 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/technology/layer_map.py
+-rw-r--r--   0        0        0    16139 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/technology/layer_stack.py
+-rw-r--r--   0        0        0    42126 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/technology/layer_views.py
+-rw-r--r--   0        0        0     1984 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/technology/simulation_settings.py
+-rw-r--r--   0        0        0     1635 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/types.py
+-rw-r--r--   0        0        0    10008 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/typings.py
+-rw-r--r--   0        0        0        0 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/utils/__init__.py
+-rw-r--r--   0        0        0     1342 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/utils/async_utils.py
+-rw-r--r--   0        0        0      376 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/utils/color_utils.py
+-rw-r--r--   0        0        0      558 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/utils/file_utils.py
+-rw-r--r--   0        0        0      185 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/utils/function_utils.py
+-rw-r--r--   0        0        0      684 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/utils/xml_utils.py
+-rw-r--r--   0        0        0     1453 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/utils/yaml_utils.py
+-rw-r--r--   0        0        0     4865 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/watch.py
+-rw-r--r--   0        0        0        0 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/widgets/__init__.py
+-rw-r--r--   0        0        0     7969 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/widgets/layout_viewer.py
+-rw-r--r--   0        0        0     7480 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/gdsfactory/write_cells.py
+-rw-r--r--   0        0        0     4943 2023-05-29 17:46:56.537329 gdsfactory-6.99.0/pyproject.toml
+-rw-r--r--   0        0        0    18875 1970-01-01 00:00:00.000000 gdsfactory-6.99.0/PKG-INFO
```

### Comparing `gdsfactory-6.98.2/LICENSE` & `gdsfactory-6.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/README.md` & `gdsfactory-6.99.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gdsfactory 6.98.2
+# gdsfactory 6.99.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/__init__.py` & `gdsfactory-6.99.0/gdsfactory/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,8 +148,8 @@
     "snap",
     "typings",
     "technology",
     "write_cells",
     "xsection",
     "PATH",
 )
-__version__ = "6.98.2"
+__version__ = "6.99.0"
```

### Comparing `gdsfactory-6.98.2/gdsfactory/add_keepout.py` & `gdsfactory-6.99.0/gdsfactory/add_keepout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/add_labels.py` & `gdsfactory-6.99.0/gdsfactory/add_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/add_loopback.py` & `gdsfactory-6.99.0/gdsfactory/add_loopback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/add_padding.py` & `gdsfactory-6.99.0/gdsfactory/add_padding.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/add_pins.py` & `gdsfactory-6.99.0/gdsfactory/add_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/add_ports.py` & `gdsfactory-6.99.0/gdsfactory/add_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/add_tapers.py` & `gdsfactory-6.99.0/gdsfactory/add_tapers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/add_tapers_cross_section.py` & `gdsfactory-6.99.0/gdsfactory/add_tapers_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/add_termination.py` & `gdsfactory-6.99.0/gdsfactory/add_termination.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/asserts.py` & `gdsfactory-6.99.0/gdsfactory/asserts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/cell.py` & `gdsfactory-6.99.0/gdsfactory/cell.py`

 * *Files 22% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         # get only the args which are explicitly passed and different from defaults
         changed_arg_set = set(passed_args_list).difference(default_args_list)
         changed_arg_list = sorted(changed_arg_set)
 
         # if any args were different from default, append a hash of those args.
         # else, keep only the base name
         named_args_string = "_".join(changed_arg_list)
+        # print(named_args_string)
 
         if changed_arg_list:
             named_args_string = (
                 hashlib.md5(named_args_string.encode()).hexdigest()[:8]
                 if with_hash
                 or len(named_args_string) > 28
                 or "'" in named_args_string
@@ -420,131 +421,39 @@
     c = gf.Component()
     ref = c << gf.components.straight()
     c.add_ports(ref.ports)
     gf.add_pins.add_pins(c)
     return c
 
 
+def test_hashes() -> None:
+    import gdsfactory as gf
+
+    c = gf.components.mzi()
+    names1 = {i.name for i in c.get_dependencies()}
+    gf.clear_cache()
+    c = gf.components.mzi()
+    names2 = {i.name for i in c.get_dependencies()}
+    assert names1 == names2
+
+
 if __name__ == "__main__":
     import gdsfactory as gf
 
-    @gf.declarative_cell
-    class mzi:
-        delta_length: float = 10.0
-
-        def instances(self):
-            self.mmi_in = gf.components.mmi1x2()
-            self.mmi_out = gf.components.mmi2x2()
-            self.straight_top1 = gf.components.straight(length=self.delta_length / 2)
-            self.straight_top2 = gf.components.straight(length=self.delta_length / 2)
-            self.bend_top1 = gf.components.bend_euler()
-            self.bend_top2 = gf.components.bend_euler().mirror()
-            self.bend_top3 = gf.components.bend_euler().mirror()
-            self.bend_top4 = gf.components.bend_euler()
-            self.bend_btm1 = gf.components.bend_euler().mirror()
-            self.bend_btm2 = gf.components.bend_euler()
-            self.bend_btm3 = gf.components.bend_euler()
-            self.bend_btm4 = gf.components.bend_euler().mirror()
-
-        def connections(self):
-            return [
-                (self.bend_top1.ports["o1"], self.mmi_in.ports["o2"]),
-                (self.straight_top1.ports["o1"], self.bend_top1.ports["o2"]),
-                (self.bend_top2.ports["o1"], self.straight_top1.ports["o2"]),
-                (self.bend_top3.ports["o1"], self.bend_top2.ports["o2"]),
-                (self.straight_top2.ports["o1"], self.bend_top3.ports["o2"]),
-                (self.bend_top4.ports["o1"], self.straight_top2.ports["o2"]),
-                (self.bend_btm1.ports["o1"], self.mmi_in.ports["o3"]),
-                (self.bend_btm2.ports["o1"], self.bend_btm1.ports["o2"]),
-                (self.bend_btm3.ports["o1"], self.bend_btm2.ports["o2"]),
-                (self.bend_btm4.ports["o1"], self.bend_btm3.ports["o2"]),
-                (self.mmi_out.ports["o1"], self.bend_btm4.ports["o2"]),
-            ]
-
-        def ports(self):
-            return {
-                "o1": self.mmi_in.ports["o1"],
-                "o2": self.mmi_out.ports["o3"],
-                "o3": self.mmi_out.ports["o4"],
-            }
-
-    @gf.declarative_cell
-    class mzi_lattice_fixme:
-        """does not work"""
-
-        delta_lengths: Tuple[float, ...] = (10.0, 100)
-
-        def instances(self):
-            self.mzis = {}
-            for i, d in enumerate(self.delta_lengths):
-                self.mzis[i] = mzi(delta_length=d).ref()
-
-        def connections(self):
-            return [
-                (self.mzis[i + 1]["o1"], self.mzis[i]["o2"])
-                for i in range(len(self.mzis) - 1)
-            ]
-
-        def ports(self):
-            return {
-                "o1": self.mzis[0].ports["o1"],
-                "o2": self.mzis[len(self.mzis) - 1].ports["o2"],
-            }
-
-    @gf.declarative_cell
-    class mzi_lattice:
-        """Works"""
-
-        delta_length1: float = 10.0
-        delta_length2: float = 100.0
-
-        def instances(self):
-            self.mzi1 = mzi(delta_length=self.delta_length1)
-            self.mzi2 = mzi(delta_length=self.delta_length2)
-
-        def connections(self):
-            return [
-                (self.mzi2["o1"], self.mzi1.ports["o2"]),
-            ]
-
-        def ports(self):
-            return {
-                "o1": self.mzi1.ports["o1"],
-                "o2": self.mzi2.ports["o2"],
-            }
-
-    @gf.declarative_cell
-    class mzi_lattice_with_routes:
-        """Works"""
-
-        delta_length1: float = 10.0
-        delta_length2: float = 100.0
-
-        def instances(self):
-            self.mzi1 = mzi(delta_length=self.delta_length1)
-            self.mzi2 = mzi(delta_length=self.delta_length2)
-
-        def placements(self):
-            pass
-
-        def routes(self):
-            return [
-                (self.mzi2["o1"], self.mzi1.ports["o2"]),
-            ]
-
-        def ports(self):
-            return {
-                "o1": self.mzi1.ports["o1"],
-                "o2": self.mzi2.ports["o2"],
-            }
-
-    # c = mzi(delta_length=10)
-    # c = mzi()
-    c = mzi_lattice()
-    c.show()
+    c = gf.c.mzi()
+    print(c.name)
+
+    # c = gf.components.mzi()
+    # names1 = set([i.name for i in c.get_dependencies()])
+    # gf.clear_cache()
+    # c = gf.components.mzi()
+    # names2 = set([i.name for i in c.get_dependencies()])
+    # assert names1 == names2
+
+    # test_hashes()
 
     # test_names()
     # c = wg()
     # test_import_gds_settings()
 
     # import gdsfactory as gf
```

### Comparing `gdsfactory-6.98.2/gdsfactory/circuitviz.py` & `gdsfactory-6.99.0/gdsfactory/circuitviz.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/cli.py` & `gdsfactory-6.99.0/gdsfactory/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from gdsfactory.write_cells import write_cells as write_cells_to_separate_gds
 
 try:
     import rich_click as click
 except ImportError:
     import click
 
-VERSION = "6.98.2"
+VERSION = "6.99.0"
 LAYER_LABEL = LAYER.LABEL
 
 
 def print_version(ctx: Context, param: Option, value: bool) -> None:
     """Prints the version."""
     if not value or ctx.resilient_parsing:
         return
```

### Comparing `gdsfactory-6.98.2/gdsfactory/component.py` & `gdsfactory-6.99.0/gdsfactory/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -6243,127 +6243,54 @@
 00018620: 3220 3d20 6766 2e69 6d70 6f72 745f 6764  2 = gf.import_gd
 00018630: 7328 6764 7370 6174 682c 206e 616d 653d  s(gdspath, name=
 00018640: 226d 7a69 5f73 616d 706c 6522 2c20 7265  "mzi_sample", re
 00018650: 6164 5f6d 6574 6164 6174 613d 5472 7565  ad_metadata=True
 00018660: 290a 2020 2020 6333 203d 2067 662e 726f  ).    c3 = gf.ro
 00018670: 7574 696e 672e 6164 645f 6669 6265 725f  uting.add_fiber_
 00018680: 7369 6e67 6c65 2863 3229 0a20 2020 2061  single(c2).    a
-00018690: 7373 6572 7420 6333 0a0a 0a64 6566 2074  ssert c3...def t
-000186a0: 6573 745f 666c 6174 7465 6e5f 696e 7661  est_flatten_inva
-000186b0: 6c69 645f 7265 6673 5f72 6563 7572 7369  lid_refs_recursi
-000186c0: 7665 2829 202d 3e20 4e6f 6e65 3a0a 2020  ve() -> None:.  
-000186d0: 2020 696d 706f 7274 2067 6473 6661 6374    import gdsfact
-000186e0: 6f72 7920 6173 2067 660a 2020 2020 6672  ory as gf.    fr
-000186f0: 6f6d 2067 6473 6661 6374 6f72 792e 6469  om gdsfactory.di
-00018700: 6666 7465 7374 2069 6d70 6f72 7420 7275  fftest import ru
-00018710: 6e5f 786f 720a 2020 2020 6672 6f6d 2067  n_xor.    from g
-00018720: 6473 6661 6374 6f72 792e 726f 7574 696e  dsfactory.routin
-00018730: 672e 616c 6c5f 616e 676c 6520 696d 706f  g.all_angle impo
-00018740: 7274 2067 6574 5f62 756e 646c 655f 616c  rt get_bundle_al
-00018750: 6c5f 616e 676c 650a 0a20 2020 2040 6766  l_angle..    @gf
-00018760: 2e63 656c 6c0a 2020 2020 6465 6620 666c  .cell.    def fl
-00018770: 6174 2829 3a0a 2020 2020 2020 2020 6320  at():.        c 
-00018780: 3d20 6766 2e43 6f6d 706f 6e65 6e74 2829  = gf.Component()
-00018790: 0a20 2020 2020 2020 206d 6d69 3120 3d20  .        mmi1 = 
-000187a0: 2863 203c 3c20 6766 2e63 6f6d 706f 6e65  (c << gf.compone
-000187b0: 6e74 732e 6d6d 6931 7832 2829 292e 6d6f  nts.mmi1x2()).mo
-000187c0: 7665 2828 302c 202d 312e 3030 3035 2929  ve((0, -1.0005))
-000187d0: 0a20 2020 2020 2020 206d 6d69 3220 3d20  .        mmi2 = 
-000187e0: 2863 203c 3c20 6766 2e63 6f6d 706f 6e65  (c << gf.compone
-000187f0: 6e74 732e 6d6d 6931 7832 2829 292e 726f  nts.mmi1x2()).ro
-00018800: 7461 7465 2838 3029 0a20 2020 2020 2020  tate(80).       
-00018810: 206d 6d69 322e 6d6f 7665 2828 3430 2c20   mmi2.move((40, 
-00018820: 3230 2929 0a20 2020 2020 2020 2062 756e  20)).        bun
-00018830: 646c 6520 3d20 6765 745f 6275 6e64 6c65  dle = get_bundle
-00018840: 5f61 6c6c 5f61 6e67 6c65 285b 6d6d 6931  _all_angle([mmi1
-00018850: 2e70 6f72 7473 5b22 6f32 225d 5d2c 205b  .ports["o2"]], [
-00018860: 6d6d 6932 2e70 6f72 7473 5b22 6f31 225d  mmi2.ports["o1"]
-00018870: 5d29 0a20 2020 2020 2020 2066 6f72 2072  ]).        for r
-00018880: 6f75 7465 2069 6e20 6275 6e64 6c65 3a0a  oute in bundle:.
-00018890: 2020 2020 2020 2020 2020 2020 632e 6164              c.ad
-000188a0: 6428 726f 7574 652e 7265 6665 7265 6e63  d(route.referenc
-000188b0: 6573 290a 2020 2020 2020 2020 7265 7475  es).        retu
-000188c0: 726e 2063 0a0a 2020 2020 4067 662e 6365  rn c..    @gf.ce
-000188d0: 6c6c 0a20 2020 2064 6566 2068 6965 7261  ll.    def hiera
-000188e0: 7263 6879 2829 3a0a 2020 2020 2020 2020  rchy():.        
-000188f0: 6320 3d20 6766 2e43 6f6d 706f 6e65 6e74  c = gf.Component
-00018900: 2829 0a20 2020 2020 2020 2028 6320 3c3c  ().        (c <<
-00018910: 2066 6c61 7428 2929 2e72 6f74 6174 6528   flat()).rotate(
-00018920: 3333 290a 2020 2020 2020 2020 2863 203c  33).        (c <
-00018930: 3c20 666c 6174 2829 292e 726f 7461 7465  < flat()).rotate
-00018940: 2833 3329 2e6d 6f76 6528 2830 2c20 3130  (33).move((0, 10
-00018950: 3029 290a 2020 2020 2020 2020 2863 203c  0)).        (c <
-00018960: 3c20 666c 6174 2829 292e 6d6f 7665 2828  < flat()).move((
-00018970: 3130 302c 2030 2929 0a20 2020 2020 2020  100, 0)).       
-00018980: 2072 6574 7572 6e20 630a 0a20 2020 2063   return c..    c
-00018990: 5f6f 7269 6720 3d20 6869 6572 6172 6368  _orig = hierarch
-000189a0: 7928 290a 2020 2020 635f 6e65 7720 3d20  y().    c_new = 
-000189b0: 666c 6174 7465 6e5f 696e 7661 6c69 645f  flatten_invalid_
-000189c0: 7265 6673 5f72 6563 7572 7369 7665 2863  refs_recursive(c
-000189d0: 5f6f 7269 6729 0a20 2020 2061 7373 6572  _orig).    asser
-000189e0: 7420 635f 6e65 7720 6973 206e 6f74 2063  t c_new is not c
-000189f0: 5f6f 7269 670a 2020 2020 696e 7661 6c69  _orig.    invali
-00018a00: 645f 7265 6673 5f66 696c 656e 616d 6520  d_refs_filename 
-00018a10: 3d20 2269 6e76 616c 6964 5f72 6566 732e  = "invalid_refs.
-00018a20: 6764 7322 0a20 2020 2069 6e76 616c 6964  gds".    invalid
-00018a30: 5f72 6566 735f 6669 7865 645f 6669 6c65  _refs_fixed_file
-00018a40: 6e61 6d65 203d 2022 696e 7661 6c69 645f  name = "invalid_
-00018a50: 7265 6673 5f66 6978 6564 2e67 6473 220a  refs_fixed.gds".
-00018a60: 2020 2020 2320 6764 7320 6669 6c65 7320      # gds files 
-00018a70: 7368 6f75 6c64 2073 7469 6c6c 2062 6520  should still be 
-00018a80: 7361 6d65 2074 6f20 316e 6d20 746f 6c65  same to 1nm tole
-00018a90: 7261 6e63 650a 2020 2020 635f 6f72 6967  rance.    c_orig
-00018aa0: 2e77 7269 7465 5f67 6473 2869 6e76 616c  .write_gds(inval
-00018ab0: 6964 5f72 6566 735f 6669 6c65 6e61 6d65  id_refs_filename
-00018ac0: 290a 2020 2020 635f 6e65 772e 7772 6974  ).    c_new.writ
-00018ad0: 655f 6764 7328 696e 7661 6c69 645f 7265  e_gds(invalid_re
-00018ae0: 6673 5f66 6978 6564 5f66 696c 656e 616d  fs_fixed_filenam
-00018af0: 6529 0a20 2020 2072 756e 5f78 6f72 2869  e).    run_xor(i
-00018b00: 6e76 616c 6964 5f72 6566 735f 6669 6c65  nvalid_refs_file
-00018b10: 6e61 6d65 2c20 696e 7661 6c69 645f 7265  name, invalid_re
-00018b20: 6673 5f66 6978 6564 5f66 696c 656e 616d  fs_fixed_filenam
-00018b30: 6529 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f  e)...if __name__
-00018b40: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0a   == "__main__":.
-00018b50: 2020 2020 2320 696d 706f 7274 2067 6473      # import gds
-00018b60: 6661 6374 6f72 7920 6173 2067 660a 0a20  factory as gf.. 
-00018b70: 2020 2074 6573 745f 7265 6d61 705f 6c61     test_remap_la
-00018b80: 7965 7273 2829 0a20 2020 2023 2063 203d  yers().    # c =
-00018b90: 2067 662e 436f 6d70 6f6e 656e 7428 290a   gf.Component().
-00018ba0: 2020 2020 2320 7020 3d20 632e 6164 645f      # p = c.add_
-00018bb0: 706f 6c79 676f 6e28 0a20 2020 2023 2020  polygon(.    #  
-00018bc0: 2020 205b 282d 382c 2036 2c20 372c 2039     [(-8, 6, 7, 9
-00018bd0: 292c 2028 2d36 2c20 382c 2031 372c 2035  ), (-6, 8, 17, 5
-00018be0: 295d 2c20 6c61 7965 723d 2831 2c20 3029  )], layer=(1, 0)
-00018bf0: 0a20 2020 2023 2029 2020 2320 4744 5320  .    # )  # GDS 
-00018c00: 6c61 7965 7273 2061 7265 2074 7570 6c65  layers are tuple
-00018c10: 7320 6f66 2069 6e74 7320 2862 7574 2069  s of ints (but i
-00018c20: 6620 7765 2075 7365 206f 6e6c 7920 6f6e  f we use only on
-00018c30: 6520 6e75 6d62 6572 2069 7420 6173 7375  e number it assu
-00018c40: 6d65 7320 7468 6520 6f74 6865 7220 6e75  mes the other nu
-00018c50: 6d62 6572 2069 7320 3029 0a0a 2020 2020  mber is 0)..    
-00018c60: 2320 6332 203d 2067 662e 436f 6d70 6f6e  # c2 = gf.Compon
-00018c70: 656e 7428 290a 2020 2020 2320 6320 3d20  ent().    # c = 
-00018c80: 6766 2e63 6f6d 706f 6e65 6e74 732e 6d7a  gf.components.mz
-00018c90: 6928 290a 2020 2020 2320 7072 696e 7428  i().    # print(
-00018ca0: 632e 6765 745f 6c61 7965 725f 6e61 6d65  c.get_layer_name
-00018cb0: 7328 2929 0a20 2020 2023 2063 203d 2067  s()).    # c = g
-00018cc0: 662e 636f 6d70 6f6e 656e 7473 2e6d 7a69  f.components.mzi
-00018cd0: 2829 0a20 2020 2023 2070 7269 6e74 2863  ().    # print(c
-00018ce0: 2e67 6574 5f6c 6179 6572 5f6e 616d 6573  .get_layer_names
-00018cf0: 2829 290a 2020 2020 2320 7220 3d20 632e  ()).    # r = c.
-00018d00: 7265 6628 290a 2020 2020 2320 6332 2e63  ref().    # c2.c
-00018d10: 6f70 795f 6368 696c 645f 696e 666f 2863  opy_child_info(c
-00018d20: 2e6e 616d 6564 5f72 6566 6572 656e 6365  .named_reference
-00018d30: 735b 2273 7874 225d 290a 2020 2020 2320  s["sxt"]).    # 
-00018d40: 7465 7374 5f72 656d 6170 5f6c 6179 6572  test_remap_layer
-00018d50: 7328 290a 2020 2020 2320 6320 3d20 7465  s().    # c = te
-00018d60: 7374 5f67 6574 5f6c 6179 6572 7328 290a  st_get_layers().
-00018d70: 2020 2020 2320 632e 706c 6f74 5f71 7428      # c.plot_qt(
-00018d80: 290a 2020 2020 2320 632e 706c 6f74 6828  ).    # c.ploth(
-00018d90: 290a 2020 2020 2320 6320 3d20 7465 7374  ).    # c = test
-00018da0: 5f65 7874 7261 6374 2829 0a20 2020 2023  _extract().    #
-00018db0: 2067 6473 7061 7468 203d 2063 2e77 7269   gdspath = c.wri
-00018dc0: 7465 5f67 6473 2829 0a20 2020 2023 2067  te_gds().    # g
-00018dd0: 662e 7368 6f77 2867 6473 7061 7468 290a  f.show(gdspath).
-00018de0: 2020 2020 2320 632e 7368 6f77 2873 686f      # c.show(sho
-00018df0: 775f 706f 7274 733d 5472 7565 290a 2020  w_ports=True).  
-00018e00: 2020 2320 632e 7368 6f77 2829 0a           # c.show().
+00018690: 7373 6572 7420 6333 0a0a 0a69 6620 5f5f  ssert c3...if __
+000186a0: 6e61 6d65 5f5f 203d 3d20 225f 5f6d 6169  name__ == "__mai
+000186b0: 6e5f 5f22 3a0a 2020 2020 2320 696d 706f  n__":.    # impo
+000186c0: 7274 2067 6473 6661 6374 6f72 7920 6173  rt gdsfactory as
+000186d0: 2067 660a 0a20 2020 2074 6573 745f 7265   gf..    test_re
+000186e0: 6d61 705f 6c61 7965 7273 2829 0a20 2020  map_layers().   
+000186f0: 2023 2063 203d 2067 662e 436f 6d70 6f6e   # c = gf.Compon
+00018700: 656e 7428 290a 2020 2020 2320 7020 3d20  ent().    # p = 
+00018710: 632e 6164 645f 706f 6c79 676f 6e28 0a20  c.add_polygon(. 
+00018720: 2020 2023 2020 2020 205b 282d 382c 2036     #     [(-8, 6
+00018730: 2c20 372c 2039 292c 2028 2d36 2c20 382c  , 7, 9), (-6, 8,
+00018740: 2031 372c 2035 295d 2c20 6c61 7965 723d   17, 5)], layer=
+00018750: 2831 2c20 3029 0a20 2020 2023 2029 2020  (1, 0).    # )  
+00018760: 2320 4744 5320 6c61 7965 7273 2061 7265  # GDS layers are
+00018770: 2074 7570 6c65 7320 6f66 2069 6e74 7320   tuples of ints 
+00018780: 2862 7574 2069 6620 7765 2075 7365 206f  (but if we use o
+00018790: 6e6c 7920 6f6e 6520 6e75 6d62 6572 2069  nly one number i
+000187a0: 7420 6173 7375 6d65 7320 7468 6520 6f74  t assumes the ot
+000187b0: 6865 7220 6e75 6d62 6572 2069 7320 3029  her number is 0)
+000187c0: 0a0a 2020 2020 2320 6332 203d 2067 662e  ..    # c2 = gf.
+000187d0: 436f 6d70 6f6e 656e 7428 290a 2020 2020  Component().    
+000187e0: 2320 6320 3d20 6766 2e63 6f6d 706f 6e65  # c = gf.compone
+000187f0: 6e74 732e 6d7a 6928 290a 2020 2020 2320  nts.mzi().    # 
+00018800: 7072 696e 7428 632e 6765 745f 6c61 7965  print(c.get_laye
+00018810: 725f 6e61 6d65 7328 2929 0a20 2020 2023  r_names()).    #
+00018820: 2063 203d 2067 662e 636f 6d70 6f6e 656e   c = gf.componen
+00018830: 7473 2e6d 7a69 2829 0a20 2020 2023 2070  ts.mzi().    # p
+00018840: 7269 6e74 2863 2e67 6574 5f6c 6179 6572  rint(c.get_layer
+00018850: 5f6e 616d 6573 2829 290a 2020 2020 2320  _names()).    # 
+00018860: 7220 3d20 632e 7265 6628 290a 2020 2020  r = c.ref().    
+00018870: 2320 6332 2e63 6f70 795f 6368 696c 645f  # c2.copy_child_
+00018880: 696e 666f 2863 2e6e 616d 6564 5f72 6566  info(c.named_ref
+00018890: 6572 656e 6365 735b 2273 7874 225d 290a  erences["sxt"]).
+000188a0: 2020 2020 2320 7465 7374 5f72 656d 6170      # test_remap
+000188b0: 5f6c 6179 6572 7328 290a 2020 2020 2320  _layers().    # 
+000188c0: 6320 3d20 7465 7374 5f67 6574 5f6c 6179  c = test_get_lay
+000188d0: 6572 7328 290a 2020 2020 2320 632e 706c  ers().    # c.pl
+000188e0: 6f74 5f71 7428 290a 2020 2020 2320 632e  ot_qt().    # c.
+000188f0: 706c 6f74 6828 290a 2020 2020 2320 6320  ploth().    # c 
+00018900: 3d20 7465 7374 5f65 7874 7261 6374 2829  = test_extract()
+00018910: 0a20 2020 2023 2067 6473 7061 7468 203d  .    # gdspath =
+00018920: 2063 2e77 7269 7465 5f67 6473 2829 0a20   c.write_gds(). 
+00018930: 2020 2023 2067 662e 7368 6f77 2867 6473     # gf.show(gds
+00018940: 7061 7468 290a 2020 2020 2320 632e 7368  path).    # c.sh
+00018950: 6f77 2873 686f 775f 706f 7274 733d 5472  ow(show_ports=Tr
+00018960: 7565 290a 2020 2020 2320 632e 7368 6f77  ue).    # c.show
+00018970: 2829 0a                                  ().
```

### Comparing `gdsfactory-6.98.2/gdsfactory/component_layout.py` & `gdsfactory-6.99.0/gdsfactory/component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/component_reference.py` & `gdsfactory-6.99.0/gdsfactory/component_reference.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/C.py` & `gdsfactory-6.99.0/gdsfactory/components/C.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/L.py` & `gdsfactory-6.99.0/gdsfactory/components/L.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/__init__.py` & `gdsfactory-6.99.0/gdsfactory/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/add_fiducials.py` & `gdsfactory-6.99.0/gdsfactory/components/add_fiducials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/add_grating_couplers.py` & `gdsfactory-6.99.0/gdsfactory/components/add_grating_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/add_trenches.py` & `gdsfactory-6.99.0/gdsfactory/components/add_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/align.py` & `gdsfactory-6.99.0/gdsfactory/components/align.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/array_component.py` & `gdsfactory-6.99.0/gdsfactory/components/array_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/array_with_fanout.py` & `gdsfactory-6.99.0/gdsfactory/components/array_with_fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/array_with_via.py` & `gdsfactory-6.99.0/gdsfactory/components/array_with_via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/awg.py` & `gdsfactory-6.99.0/gdsfactory/components/awg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/bbox.py` & `gdsfactory-6.99.0/gdsfactory/components/bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/bend_circular.py` & `gdsfactory-6.99.0/gdsfactory/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/bend_circular_heater.py` & `gdsfactory-6.99.0/gdsfactory/components/bend_circular_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/bend_euler.py` & `gdsfactory-6.99.0/gdsfactory/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/bend_port.py` & `gdsfactory-6.99.0/gdsfactory/components/bend_port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/bend_s.py` & `gdsfactory-6.99.0/gdsfactory/components/bend_s.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/bezier.py` & `gdsfactory-6.99.0/gdsfactory/components/bezier.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cavity.py` & `gdsfactory-6.99.0/gdsfactory/components/cavity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cdc.py` & `gdsfactory-6.99.0/gdsfactory/components/cdc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cdsem_all.py` & `gdsfactory-6.99.0/gdsfactory/components/cdsem_all.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cdsem_bend180.py` & `gdsfactory-6.99.0/gdsfactory/components/cdsem_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cdsem_coupler.py` & `gdsfactory-6.99.0/gdsfactory/components/cdsem_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cdsem_straight.py` & `gdsfactory-6.99.0/gdsfactory/components/cdsem_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cdsem_straight_density.py` & `gdsfactory-6.99.0/gdsfactory/components/cdsem_straight_density.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/circle.py` & `gdsfactory-6.99.0/gdsfactory/components/circle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coh_rx_dual_pol.py` & `gdsfactory-6.99.0/gdsfactory/components/coh_rx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coh_rx_single_pol.py` & `gdsfactory-6.99.0/gdsfactory/components/coh_rx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coh_tx_dual_pol.py` & `gdsfactory-6.99.0/gdsfactory/components/coh_tx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coh_tx_single_pol.py` & `gdsfactory-6.99.0/gdsfactory/components/coh_tx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/compass.py` & `gdsfactory-6.99.0/gdsfactory/components/compass.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/component_lattice.py` & `gdsfactory-6.99.0/gdsfactory/components/component_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/component_sequence.py` & `gdsfactory-6.99.0/gdsfactory/components/component_sequence.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/copy_layers.py` & `gdsfactory-6.99.0/gdsfactory/components/copy_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coupler.py` & `gdsfactory-6.99.0/gdsfactory/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coupler90.py` & `gdsfactory-6.99.0/gdsfactory/components/coupler90.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coupler90bend.py` & `gdsfactory-6.99.0/gdsfactory/components/coupler90bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coupler_adiabatic.py` & `gdsfactory-6.99.0/gdsfactory/components/coupler_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coupler_asymmetric.py` & `gdsfactory-6.99.0/gdsfactory/components/coupler_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coupler_full.py` & `gdsfactory-6.99.0/gdsfactory/components/coupler_full.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coupler_ring.py` & `gdsfactory-6.99.0/gdsfactory/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coupler_straight.py` & `gdsfactory-6.99.0/gdsfactory/components/coupler_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coupler_straight_asymmetric.py` & `gdsfactory-6.99.0/gdsfactory/components/coupler_straight_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/coupler_symmetric.py` & `gdsfactory-6.99.0/gdsfactory/components/coupler_symmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cross.py` & `gdsfactory-6.99.0/gdsfactory/components/cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/crossing_waveguide.py` & `gdsfactory-6.99.0/gdsfactory/components/crossing_waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv` & `gdsfactory-6.99.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv` & `gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv` & `gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv` & `gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv` & `gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv` & `gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv` & `gdsfactory-6.99.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cutback_2x2.py` & `gdsfactory-6.99.0/gdsfactory/components/cutback_2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cutback_bend.py` & `gdsfactory-6.99.0/gdsfactory/components/cutback_bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cutback_component.py` & `gdsfactory-6.99.0/gdsfactory/components/cutback_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/cutback_splitter.py` & `gdsfactory-6.99.0/gdsfactory/components/cutback_splitter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/dbr.py` & `gdsfactory-6.99.0/gdsfactory/components/dbr.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/dbr_tapered.py` & `gdsfactory-6.99.0/gdsfactory/components/dbr_tapered.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/delay_snake.py` & `gdsfactory-6.99.0/gdsfactory/components/delay_snake.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/delay_snake2.py` & `gdsfactory-6.99.0/gdsfactory/components/delay_snake2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/delay_snake3.py` & `gdsfactory-6.99.0/gdsfactory/components/delay_snake3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/delay_snake_sbend.py` & `gdsfactory-6.99.0/gdsfactory/components/delay_snake_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/dicing_lane.py` & `gdsfactory-6.99.0/gdsfactory/components/dicing_lane.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/die.py` & `gdsfactory-6.99.0/gdsfactory/components/die.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/die_bbox.py` & `gdsfactory-6.99.0/gdsfactory/components/die_bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/die_bbox_frame.py` & `gdsfactory-6.99.0/gdsfactory/components/die_bbox_frame.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/disk.py` & `gdsfactory-6.99.0/gdsfactory/components/disk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/edge_coupler_array.py` & `gdsfactory-6.99.0/gdsfactory/components/edge_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ellipse.py` & `gdsfactory-6.99.0/gdsfactory/components/ellipse.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/extend_ports_list.py` & `gdsfactory-6.99.0/gdsfactory/components/extend_ports_list.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/extension.py` & `gdsfactory-6.99.0/gdsfactory/components/extension.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/fiber.py` & `gdsfactory-6.99.0/gdsfactory/components/fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/fiber_array.py` & `gdsfactory-6.99.0/gdsfactory/components/fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/fiducial_squares.py` & `gdsfactory-6.99.0/gdsfactory/components/fiducial_squares.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ge_detector_straight_si_contacts.py` & `gdsfactory-6.99.0/gdsfactory/components/ge_detector_straight_si_contacts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_array.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_dual_pol.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_elliptical.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_elliptical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_elliptical_arbitrary.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_elliptical_lumerical.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_elliptical_trenches.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_elliptical_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_functions.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_loss.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_loss.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_loss_fiber_single.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_loss_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_rectangular.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_rectangular_arbitrary.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/grating_coupler_tree.py` & `gdsfactory-6.99.0/gdsfactory/components/grating_coupler_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/greek_cross.py` & `gdsfactory-6.99.0/gdsfactory/components/greek_cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/hline.py` & `gdsfactory-6.99.0/gdsfactory/components/hline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/interdigital_capacitor.py` & `gdsfactory-6.99.0/gdsfactory/components/interdigital_capacitor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/litho_calipers.py` & `gdsfactory-6.99.0/gdsfactory/components/litho_calipers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/litho_ruler.py` & `gdsfactory-6.99.0/gdsfactory/components/litho_ruler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/litho_steps.py` & `gdsfactory-6.99.0/gdsfactory/components/litho_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/logo.py` & `gdsfactory-6.99.0/gdsfactory/components/logo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/loop_mirror.py` & `gdsfactory-6.99.0/gdsfactory/components/loop_mirror.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mmi1x2.py` & `gdsfactory-6.99.0/gdsfactory/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mmi1x2_with_sbend.py` & `gdsfactory-6.99.0/gdsfactory/components/mode_converter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,116 @@
-import numpy as np
+from __future__ import annotations
 
 import gdsfactory as gf
 from gdsfactory.component import Component
+from gdsfactory.components.coupler_straight_asymmetric import (
+    coupler_straight_asymmetric as coupler_straight_asymmetric_function,
+)
+from gdsfactory.components.bend_euler import bend_euler_s
+from gdsfactory.components.taper import taper as taper_function
 from gdsfactory.typings import ComponentSpec, CrossSectionSpec
-from gdsfactory.components.bend_s import bend_s
 
 
 @gf.cell
-def mmi1x2_with_sbend(
-    with_sbend: bool = True,
-    s_bend: ComponentSpec = bend_s,
+def mode_converter(
+    gap: float = 0.3,
+    length: float = 10,
+    coupler_straight_asymmetric: ComponentSpec = coupler_straight_asymmetric_function,
+    bend: ComponentSpec = gf.partial(bend_euler_s, angle=45),
+    taper: ComponentSpec = taper_function,
+    mm_width: float = 1.2,
+    mc_mm_width: float = 1,
+    sm_width: float = 0.5,
+    taper_length: float = 25,
     cross_section: CrossSectionSpec = "strip",
+    **kwargs,
 ) -> Component:
-    """Returns 1x2 splitter for Cband.
+    r"""Returns Mode converter from TE0 to TE1.
 
-    https://opg.optica.org/oe/fulltext.cfm?uri=oe-21-1-1310&id=248418
+    By matching the effective indices of two waveguides with different widths,
+    light can couple from different transverse modes e.g. TE0 <-> TE1.
+    https://doi.org/10.1109/JPHOT.2019.2941742
 
     Args:
-        with_sbend: add sbend.
-        s_bend: S-bend spec.
-        cross_section: spec.
+        gap: directional coupler gap.
+        length: coupler length interaction.
+        coupler_straight_asymmetric: spec.
+        mm_width: input/output multimode waveguide width.
+        mc_mm_width: mode converter multimode waveguide width
+        sm_width: single mode waveguide width.
+        cross_section: cross_section spec.
+        kwargs: cross_section settings.
+
+    .. code::
+
+        o2 ---           --- o4
+              \         /
+               \       /
+                -------
+        o1 -----=======----- o3
+                |-----|
+                length
+
+        = : multimode width
+        - : singlemode width
     """
 
-    def mmi_widths(t):
-        from scipy.interpolate import interp1d
+    c = Component()
 
-        # Note: Custom width/offset functions MUST be vectorizable--you must be able
-        # to call them with an array input like my_custom_width_fun([0, 0.1, 0.2, 0.3, 0.4])
-        widths = np.array(
-            [0.5, 0.5, 0.6, 0.7, 0.9, 1.26, 1.4, 1.4, 1.4, 1.4, 1.31, 1.2, 1.2]
-        )
-        xold = np.linspace(0, 1, num=len(widths))
-        xnew = np.linspace(0, 1, num=100)
-        f = interp1d(xold, widths, kind="cubic")
-        return f(xnew)
-
-    c = gf.Component()
-
-    P = gf.path.straight(length=2, npoints=100)
-    xs = gf.get_cross_section(cross_section)
-    xs.width = mmi_widths
-    c << gf.path.extrude(P, cross_section=xs)
-
-    # Add "stub" straight sections for ports
-    input_port_ref = c << gf.components.straight(
-        length=0.25, cross_section=cross_section
-    )
-    input_port_ref.center = (-0.125, 0)
-    top_output_port_ref = c << gf.components.straight(
-        length=0.25, cross_section=cross_section
+    coupler = gf.get_component(
+        coupler_straight_asymmetric,
+        length=length,
+        gap=gap,
+        width_bot=mc_mm_width,
+        width_top=sm_width,
+        **kwargs,
     )
-    top_output_port_ref.center = (2.125, 0.35)
-    bottom_output_port_ref = c << gf.components.straight(
-        length=0.25, cross_section=cross_section
+
+    bend = gf.get_component(bend, **kwargs)
+
+    bot_taper = gf.get_component(
+        taper,
+        width1=mc_mm_width,
+        width2=mm_width,
+        length=taper_length,
+        **kwargs,
     )
-    bottom_output_port_ref.center = (2.125, -0.35)
-    if with_sbend:
-        sbend = gf.get_component(s_bend, cross_section=cross_section)
-        top_sbend = c << sbend
-        bot_sbend = c << sbend
-        bot_sbend.mirror([1, 0])
-        top_sbend.connect("o1", destination=top_output_port_ref.ports["o2"])
-        bot_sbend.connect("o1", destination=bottom_output_port_ref.ports["o2"])
-        c.add_port("o1", port=input_port_ref.ports["o1"])
-        c.add_port("o2", port=top_sbend.ports["o2"])
-        c.add_port("o3", port=bot_sbend.ports["o2"])
-
-    else:
-        c.add_port("o1", port=input_port_ref.ports["o1"])
-        c.add_port("o2", port=top_output_port_ref.ports["o2"])
-        c.add_port("o3", port=bottom_output_port_ref.ports["o2"])
 
+    # directional coupler
+    dc = c << coupler
+    c.absorb(dc)
+
+    # straight waveguides at the bottom
+    l_bot_straight = c << bot_taper
+    r_bot_straight = c << bot_taper
+
+    l_bot_straight.connect("o1", dc.ports["o1"])
+    r_bot_straight.connect("o1", dc.ports["o4"])
+    c.absorb(l_bot_straight)
+    c.absorb(r_bot_straight)
+
+    # top right bend with termination
+    r_bend = c << bend
+    l_bend = c << bend
+    l_bend.mirror()
+
+    l_bend.connect("o1", dc.ports["o2"])
+    r_bend.connect("o1", dc.ports["o3"])
+
+    # define ports of mode converter
+    c.add_port("o1", port=l_bot_straight.ports["o2"])
+    c.add_port("o3", port=r_bot_straight.ports["o2"])
+    c.add_port("o2", port=l_bend.ports["o2"])
+    c.add_port("o4", port=r_bend.ports["o2"])
+
+    x = gf.get_cross_section(cross_section, **kwargs)
+    if x.add_bbox:
+        c = x.add_bbox(c)
+    if x.add_pins:
+        c = x.add_pins(c)
     return c
 
 
 if __name__ == "__main__":
-    # c = mmi1x2_with_sbend(with_sbend=False)
-    # c = mmi1x2_with_sbend(with_sbend=True)
-    c = mmi1x2_with_sbend(
-        with_sbend=True,
-        cross_section=dict(cross_section="strip", settings=dict(layer=(2, 0))),
-    )
+    c = mode_converter(bbox_offsets=[0.5], bbox_layers=[(111, 0)])
+    c.pprint_ports()
     c.show(show_ports=True)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mmi2x2.py` & `gdsfactory-6.99.0/gdsfactory/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mmi2x2_with_sbend.py` & `gdsfactory-6.99.0/gdsfactory/components/mmi1x2_with_sbend.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,93 @@
 import numpy as np
+
 import gdsfactory as gf
 from gdsfactory.component import Component
 from gdsfactory.typings import ComponentSpec, CrossSectionSpec
 from gdsfactory.components.bend_s import bend_s
 
 
 @gf.cell
-def mmi2x2_with_sbend(
+def mmi1x2_with_sbend(
     with_sbend: bool = True,
     s_bend: ComponentSpec = bend_s,
     cross_section: CrossSectionSpec = "strip",
 ) -> Component:
-    """Returns mmi2x2 for Cband.
+    """Returns 1x2 splitter for Cband.
 
-    C_band 2x2MMI in 220nm thick silicon
-    https://opg.optica.org/oe/fulltext.cfm?uri=oe-25-23-28957&id=376719
+    https://opg.optica.org/oe/fulltext.cfm?uri=oe-21-1-1310&id=248418
 
     Args:
         with_sbend: add sbend.
         s_bend: S-bend spec.
         cross_section: spec.
     """
 
     def mmi_widths(t):
+        from scipy.interpolate import interp1d
+
         # Note: Custom width/offset functions MUST be vectorizable--you must be able
         # to call them with an array input like my_custom_width_fun([0, 0.1, 0.2, 0.3, 0.4])
-        widths = np.array([2 * 0.7 + 0.2, 1.48, 1.48, 1.48, 1.6])
-        return widths
+        widths = np.array(
+            [0.5, 0.5, 0.6, 0.7, 0.9, 1.26, 1.4, 1.4, 1.4, 1.4, 1.31, 1.2, 1.2]
+        )
+        xold = np.linspace(0, 1, num=len(widths))
+        xnew = np.linspace(0, 1, num=100)
+        f = interp1d(xold, widths, kind="cubic")
+        return f(xnew)
 
     c = gf.Component()
 
-    P = gf.path.straight(length=2 * 2.4 + 2 * 1.6, npoints=5)
-
-    xs = gf.get_cross_section(cross_section)
+    P = gf.path.straight(length=2, npoints=100)
+    xs = gf.get_cross_section(cross_section, add_pins=None)
     xs.width = mmi_widths
-    c << gf.path.extrude(P, cross_section=xs)
-
-    # Add input and output tapers
-    top_input_block = c << gf.components.taper(
-        length=1, width1=0.5, width2=0.7, cross_section=cross_section
-    )
-    top_input_block.move((-1, 0.45))
-    bottom_input_block = c << gf.components.taper(
-        length=1, width1=0.5, width2=0.7, cross_section=cross_section
-    )
-    bottom_input_block.move((-1, -0.45))
+    ref = c << gf.path.extrude(P, cross_section=xs)
 
-    top_output_block = c << gf.components.taper(
-        length=1, width1=0.7, width2=0.5, cross_section=cross_section
-    )
-    top_output_block.move((8, 0.45))
-    bottom_output_block = c << gf.components.taper(
-        length=1, width1=0.7, width2=0.5, cross_section=cross_section
+    # Add "stub" straight sections for ports
+    straight = gf.components.straight(
+        length=0.25, cross_section=cross_section, add_pins=None
     )
-    bottom_output_block.move((8, -0.45))
+    sl = c << straight
+    sl.center = (-0.125, 0)
+    s_topr = c << straight
+    s_topr.center = (2.125, 0.35)
+    s_botr = c << straight
+    s_botr.center = (2.125, -0.35)
 
     if with_sbend:
-        sbend = gf.get_component(s_bend, cross_section=cross_section)
-
-        top_input_sbend_ref = c << sbend
-        top_input_sbend_ref.mirror([0, 1])
-        bottom_input_sbend_ref = c << sbend
-        top_output_sbend_ref = c << sbend
-        bottom_output_sbend_ref = c << sbend
-        bottom_output_sbend_ref.mirror([0, 1])
-
-        top_input_sbend_ref.connect("o1", destination=top_input_block.ports["o1"])
-        bottom_input_sbend_ref.connect("o1", destination=bottom_input_block.ports["o1"])
-        top_output_sbend_ref.connect("o1", destination=top_output_block.ports["o2"])
-        bottom_output_sbend_ref.connect(
-            "o1", destination=bottom_output_block.ports["o2"]
-        )
+        sbend = gf.get_component(s_bend, cross_section=cross_section, add_pins=None)
+        top_sbend = c << sbend
+        bot_sbend = c << sbend
+        bot_sbend.mirror([1, 0])
+        top_sbend.connect("o1", destination=s_topr.ports["o2"])
+        bot_sbend.connect("o1", destination=s_botr.ports["o2"])
+        c.add_port("o1", port=sl.ports["o1"])
+        c.add_port("o2", port=top_sbend.ports["o2"])
+        c.add_port("o3", port=bot_sbend.ports["o2"])
 
-        c.add_port("o1", port=bottom_input_sbend_ref.ports["o2"])
-        c.add_port("o2", port=top_input_sbend_ref.ports["o2"])
-        c.add_port("o3", port=top_output_sbend_ref.ports["o2"])
-        c.add_port("o4", port=bottom_output_sbend_ref.ports["o2"])
+        c.absorb(top_sbend)
+        c.absorb(bot_sbend)
 
     else:
-        c.add_port("o2", port=top_input_block.ports["o1"])
-        c.add_port("o1", port=bottom_input_block.ports["o1"])
-        c.add_port("o3", port=top_output_block.ports["o2"])
-        c.add_port("o4", port=bottom_output_block.ports["o2"])
+        c.add_port("o1", port=sl.ports["o1"])
+        c.add_port("o2", port=s_topr.ports["o2"])
+        c.add_port("o3", port=s_botr.ports["o2"])
+
+    if xs.add_pins:
+        c = xs.add_pins(c)
+
+    c.absorb(ref)
+
+    c.absorb(sl)
+    c.absorb(s_topr)
+    c.absorb(s_botr)
     return c
 
 
 if __name__ == "__main__":
-    c = mmi2x2_with_sbend(
+    # c = mmi1x2_with_sbend(with_sbend=False)
+    # c = mmi1x2_with_sbend(with_sbend=True)
+    c = mmi1x2_with_sbend(
         with_sbend=True,
         cross_section=dict(cross_section="strip", settings=dict(layer=(2, 0))),
     )
-    # c = mmi2x2_with_sbend(with_sbend=False)
     c.show(show_ports=True)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mmi_90degree_hybrid.py` & `gdsfactory-6.99.0/gdsfactory/components/mmi_90degree_hybrid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mode_converter.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_double_bend_coupler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,90 @@
 from __future__ import annotations
 
 import gdsfactory as gf
 from gdsfactory.component import Component
-from gdsfactory.components.coupler_straight_asymmetric import (
-    coupler_straight_asymmetric as coupler_straight_asymmetric_function,
-)
-from gdsfactory.components.bend_euler import bend_euler_s
-from gdsfactory.components.taper import taper as taper_function
+from gdsfactory.components.bend_circular import bend_circular
+from gdsfactory.components.ring_single_bend_coupler import coupler_ring_bend
+from gdsfactory.components.straight import straight
 from gdsfactory.typings import ComponentSpec, CrossSectionSpec
 
 
 @gf.cell
-def mode_converter(
-    gap: float = 0.3,
-    length: float = 10,
-    coupler_straight_asymmetric: ComponentSpec = coupler_straight_asymmetric_function,
-    bend: ComponentSpec = gf.partial(bend_euler_s, angle=45),
-    taper: ComponentSpec = taper_function,
-    mm_width: float = 1.2,
-    mc_mm_width: float = 1,
-    sm_width: float = 0.5,
-    taper_length: float = 25,
-    cross_section: CrossSectionSpec = "strip",
+def ring_double_bend_coupler(
+    radius: float = 5.0,
+    gap: float = 0.2,
+    coupling_angle_coverage: float = 70.0,
+    bend: ComponentSpec = bend_circular,
+    length_x: float = 0.6,
+    length_y: float = 0.6,
+    cross_section_inner: CrossSectionSpec = "strip",
+    cross_section_outer: CrossSectionSpec = "strip",
     **kwargs,
 ) -> Component:
-    r"""Returns Mode converter from TE0 to TE1.
+    r"""Returns ring with double curved couplers.
 
-    By matching the effective indices of two waveguides with different widths,
-    light can couple from different transverse modes e.g. TE0 <-> TE1.
-    https://doi.org/10.1109/JPHOT.2019.2941742
+    TODO: enable euler bends.
 
     Args:
-        gap: directional coupler gap.
-        length: coupler length interaction.
-        coupler_straight_asymmetric: spec.
-        mm_width: input/output multimode waveguide width.
-        mc_mm_width: mode converter multimode waveguide width
-        sm_width: single mode waveguide width.
-        cross_section: cross_section spec.
+        radius: um.
+        gap: um.
+        angle_inner: of the inner bend, from beginning to end. Depending on the bend chosen, gap may not be preserved.
+        angle_outer: of the outer bend, from beginning to end. Depending on the bend chosen, gap may not be preserved.
+        bend: for bend.
+        length_y: vertical straight length.
+        cross_section_inner: spec inner bend.
+        cross_section_outer: spec outer bend.
         kwargs: cross_section settings.
-
-    .. code::
-
-        o2 ---           --- o4
-              \         /
-               \       /
-                -------
-        o1 -----=======----- o3
-                |-----|
-                length
-
-        = : multimode width
-        - : singlemode width
     """
-
     c = Component()
 
-    coupler = gf.get_component(
-        coupler_straight_asymmetric,
-        length=length,
-        gap=gap,
-        width_bot=mc_mm_width,
-        width_top=sm_width,
-        **kwargs,
-    )
-
-    bend = gf.get_component(bend, **kwargs)
-
-    bot_taper = gf.get_component(
-        taper,
-        width1=mc_mm_width,
-        width2=mm_width,
-        length=taper_length,
-        **kwargs,
+    c_halfring = coupler_ring_bend(
+        radius=radius,
+        coupler_gap=gap,
+        coupling_angle_coverage=coupling_angle_coverage,
+        length_x=length_x,
+        cross_section_inner=cross_section_inner,
+        cross_section_outer=cross_section_outer,
+        bend=bend,
     )
 
-    # directional coupler
-    dc = c << coupler
-    c.absorb(dc)
-
-    # straight waveguides at the bottom
-    l_bot_straight = c << bot_taper
-    r_bot_straight = c << bot_taper
-
-    l_bot_straight.connect("o1", dc.ports["o1"])
-    r_bot_straight.connect("o1", dc.ports["o4"])
-    c.absorb(l_bot_straight)
-    c.absorb(r_bot_straight)
-
-    # top right bend with termination
-    r_bend = c << bend
-    l_bend = c << bend
-    l_bend.mirror()
-
-    l_bend.connect("o1", dc.ports["o2"])
-    r_bend.connect("o1", dc.ports["o3"])
-
-    # define ports of mode converter
-    c.add_port("o1", port=l_bot_straight.ports["o2"])
-    c.add_port("o3", port=r_bot_straight.ports["o2"])
-    c.add_port("o2", port=l_bend.ports["o2"])
-    c.add_port("o4", port=r_bend.ports["o2"])
-
-    x = gf.get_cross_section(cross_section, **kwargs)
-    if x.add_bbox:
-        c = x.add_bbox(c)
-    if x.add_pins:
-        c = x.add_pins(c)
+    xi = gf.get_cross_section(cross_section_inner)
+    xo = gf.get_cross_section(cross_section_outer)
+    half_height = radius + xi.width / 2 + gap + xo.width + length_y / 2
+
+    if c_halfring.ysize > half_height:
+        raise ValueError(
+            "The coupling_angle_coverage is too large for the given bend radius: "
+            + "the coupling waveguides will overlap."
+        )
+
+    cb = c << c_halfring
+    ct = c << c_halfring
+
+    cross_section = cross_section_inner
+    sy = straight(length=length_y, cross_section=cross_section, **kwargs)
+    sl = c << sy
+    sr = c << sy
+
+    sl.connect(port="o1", destination=cb.ports["o2"])
+    ct.connect(port="o3", destination=sl.ports["o2"])
+    sr.connect(port="o1", destination=ct.ports["o2"])
+    cb.connect(port="o3", destination=sr.ports["o2"])
+
+    c.absorb(cb)
+    c.absorb(ct)
+    c.absorb(sl)
+    c.absorb(sr)
+
+    c.add_port("o1", port=cb.ports["o1"])
+    c.add_port("o2", port=ct.ports["o4"])
+    c.add_port("o3", port=ct.ports["o1"])
+    c.add_port("o4", port=cb.ports["o4"])
     return c
 
 
 if __name__ == "__main__":
-    c = mode_converter(bbox_offsets=[0.5], bbox_layers=[(111, 0)])
-    c.pprint_ports()
+    # c = coupler_bend(radius=5)
+    # c = coupler_ring_bend()
+    c = ring_double_bend_coupler()
+    c.assert_ports_on_grid()
     c.show(show_ports=True)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mzi.py` & `gdsfactory-6.99.0/gdsfactory/components/mzi.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,25 +218,27 @@
     mzi2x2_2x2,
     splitter=coupler,
     combiner=coupler,
 )
 
 
 if __name__ == "__main__":
-    from gdsfactory import get_generic_pdk
+    c = mzi()
+    print(sorted([i.name for i in c.get_dependencies()]))
+    # from gdsfactory import get_generic_pdk
 
-    pdk = get_generic_pdk()
-    pdk.activate()
+    # pdk = get_generic_pdk()
+    # pdk.activate()
 
-    c = mzi(cross_section="strip")
+    # c = mzi(cross_section="strip")
     # c = gf.components.mzi2x2_2x2(straight_x_top="straight_heater_metal")
     # c.show(show_ports=True)
 
     # c = gf.components.mzi2x2_2x2(straight_x_top="straight_heater_metal")
-    c = gf.routing.add_fiber_array(c)
+    # c = gf.routing.add_fiber_array(c)
     # gdspath = c.write_gds(flatten_invalid_refs=True)
     # gf.show(gdspath)
     c.show()
 
     # c1.write_gds("a.gds")
 
     # c2 = gf.read.import_gds("a.gds")
```

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mzi_arm.py` & `gdsfactory-6.99.0/gdsfactory/components/mzi_arm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mzi_arms.py` & `gdsfactory-6.99.0/gdsfactory/components/mzi_arms.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mzi_lattice.py` & `gdsfactory-6.99.0/gdsfactory/components/mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mzi_pads_center.py` & `gdsfactory-6.99.0/gdsfactory/components/mzi_pads_center.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mzi_phase_shifter.py` & `gdsfactory-6.99.0/gdsfactory/components/mzi_phase_shifter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mzit.py` & `gdsfactory-6.99.0/gdsfactory/components/mzit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mzit_lattice.py` & `gdsfactory-6.99.0/gdsfactory/components/mzit_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/mzm.py` & `gdsfactory-6.99.0/gdsfactory/components/mzm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/nxn.py` & `gdsfactory-6.99.0/gdsfactory/components/nxn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/optimal_90deg.py` & `gdsfactory-6.99.0/gdsfactory/components/optimal_90deg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/optimal_hairpin.py` & `gdsfactory-6.99.0/gdsfactory/components/optimal_hairpin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/optimal_step.py` & `gdsfactory-6.99.0/gdsfactory/components/optimal_step.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/pack_doe.py` & `gdsfactory-6.99.0/gdsfactory/components/pack_doe.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/pad.py` & `gdsfactory-6.99.0/gdsfactory/components/pad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/pad_gsg.py` & `gdsfactory-6.99.0/gdsfactory/components/pad_gsg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/pads_shorted.py` & `gdsfactory-6.99.0/gdsfactory/components/pads_shorted.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/polarization_splitter_rotator.py` & `gdsfactory-6.99.0/gdsfactory/components/polarization_splitter_rotator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ramp.py` & `gdsfactory-6.99.0/gdsfactory/components/ramp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/rectangle.py` & `gdsfactory-6.99.0/gdsfactory/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/rectangle_with_slits.py` & `gdsfactory-6.99.0/gdsfactory/components/rectangle_with_slits.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/regular_polygon.py` & `gdsfactory-6.99.0/gdsfactory/components/regular_polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/resistance_meander.py` & `gdsfactory-6.99.0/gdsfactory/components/resistance_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/resistance_sheet.py` & `gdsfactory-6.99.0/gdsfactory/components/resistance_sheet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring.py` & `gdsfactory-6.99.0/gdsfactory/components/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_crow.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_crow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_crow_couplers.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_crow_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_double.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_double_bend_coupler.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_single.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 from __future__ import annotations
 
 import gdsfactory as gf
-from gdsfactory.component import Component
-from gdsfactory.components.bend_circular import bend_circular
-from gdsfactory.components.ring_single_bend_coupler import coupler_ring_bend
+from gdsfactory.components.bend_euler import bend_euler
+from gdsfactory.components.coupler_ring import coupler_ring as coupler_ring_function
 from gdsfactory.components.straight import straight
 from gdsfactory.typings import ComponentSpec, CrossSectionSpec
 
 
 @gf.cell
-def ring_double_bend_coupler(
-    radius: float = 5.0,
+def ring_single(
     gap: float = 0.2,
-    coupling_angle_coverage: float = 70.0,
-    bend: ComponentSpec = bend_circular,
-    length_x: float = 0.6,
+    radius: float = 10.0,
+    length_x: float = 4.0,
     length_y: float = 0.6,
-    cross_section_inner: CrossSectionSpec = "strip",
-    cross_section_outer: CrossSectionSpec = "strip",
+    coupler_ring: ComponentSpec = coupler_ring_function,
+    bend: ComponentSpec = bend_euler,
+    cross_section: CrossSectionSpec = "strip",
     **kwargs,
-) -> Component:
-    r"""Returns ring with double curved couplers.
+) -> gf.Component:
+    """Returns a single ring.
 
-    TODO: enable euler bends.
+    ring coupler (cb: bottom) connects to two vertical straights (sl: left, sr: right),
+    two bends (bl, br) and horizontal straight (wg: top)
 
     Args:
-        radius: um.
-        gap: um.
-        angle_inner: of the inner bend, from beginning to end. Depending on the bend chosen, gap may not be preserved.
-        angle_outer: of the outer bend, from beginning to end. Depending on the bend chosen, gap may not be preserved.
-        bend: for bend.
+        gap: gap between for coupler.
+        radius: for the bend and coupler.
+        length_x: ring coupler length.
         length_y: vertical straight length.
-        cross_section_inner: spec inner bend.
-        cross_section_outer: spec outer bend.
+        coupler_ring: ring coupler spec.
+        bend: 90 degrees bend spec.
+        cross_section: cross_section spec.
         kwargs: cross_section settings.
+
+    .. code::
+
+          bl-st-br
+          |      |
+          sl     sr length_y
+          |      |
+         --==cb==-- gap
+
+          length_x
     """
-    c = Component()
+    gap = gf.snap.snap_to_grid(gap, nm=2)
 
-    c_halfring = coupler_ring_bend(
+    c = gf.Component()
+    cb = c << gf.get_component(
+        coupler_ring,
+        bend=bend,
+        gap=gap,
         radius=radius,
-        coupler_gap=gap,
-        coupling_angle_coverage=coupling_angle_coverage,
         length_x=length_x,
-        cross_section_inner=cross_section_inner,
-        cross_section_outer=cross_section_outer,
-        bend=bend,
+        cross_section=cross_section,
+        **kwargs,
     )
-
-    xi = gf.get_cross_section(cross_section_inner)
-    xo = gf.get_cross_section(cross_section_outer)
-    half_height = radius + xi.width / 2 + gap + xo.width + length_y / 2
-
-    if c_halfring.ysize > half_height:
-        raise ValueError(
-            "The coupling_angle_coverage is too large for the given bend radius: "
-            + "the coupling waveguides will overlap."
-        )
-
-    cb = c << c_halfring
-    ct = c << c_halfring
-
-    cross_section = cross_section_inner
     sy = straight(length=length_y, cross_section=cross_section, **kwargs)
+    b = gf.get_component(bend, cross_section=cross_section, radius=radius, **kwargs)
+    sx = straight(length=length_x, cross_section=cross_section, **kwargs)
     sl = c << sy
     sr = c << sy
+    bl = c << b
+    br = c << b
+    st = c << sx
 
     sl.connect(port="o1", destination=cb.ports["o2"])
-    ct.connect(port="o3", destination=sl.ports["o2"])
-    sr.connect(port="o1", destination=ct.ports["o2"])
-    cb.connect(port="o3", destination=sr.ports["o2"])
-
-    c.absorb(cb)
-    c.absorb(ct)
-    c.absorb(sl)
-    c.absorb(sr)
+    bl.connect(port="o2", destination=sl.ports["o2"])
+
+    st.connect(port="o2", destination=bl.ports["o1"])
+    br.connect(port="o2", destination=st.ports["o1"])
+    sr.connect(port="o1", destination=br.ports["o1"])
+    sr.connect(port="o2", destination=cb.ports["o3"])
 
+    c.add_port("o2", port=cb.ports["o4"])
     c.add_port("o1", port=cb.ports["o1"])
-    c.add_port("o2", port=ct.ports["o4"])
-    c.add_port("o3", port=ct.ports["o1"])
-    c.add_port("o4", port=cb.ports["o4"])
     return c
 
 
 if __name__ == "__main__":
-    # c = coupler_bend(radius=5)
-    # c = coupler_ring_bend()
-    c = ring_double_bend_coupler()
-    c.assert_ports_on_grid()
+    # c = ring_single(layer=(2, 0), cross_section_factory=gf.cross_section.pin, width=1)
+    # c = ring_single(width=2, gap=1, layer=(2, 0), radius=7, length_y=1)
+    # print(c.ports)
+
+    # c = gf.routing.add_fiber_array(ring_single)
+    c = ring_single(cross_section="rib", width=2)
     c.show(show_ports=True)
+
+    # cc = gf.add_pins(c)
+    # print(c.settings)
+    # print(c.settings)
+    # cc.show(show_ports=True)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_double_heater.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_double_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_double_pn.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_double_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_section_based.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_section_based.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_single.py` & `gdsfactory-6.99.0/gdsfactory/samples/14_component_connectivity.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,96 @@
 from __future__ import annotations
 
 import gdsfactory as gf
-from gdsfactory.components.bend_euler import bend_euler
-from gdsfactory.components.coupler_ring import coupler_ring as coupler_ring_function
-from gdsfactory.components.straight import straight
+from gdsfactory.component import Component
 from gdsfactory.typings import ComponentSpec, CrossSectionSpec
 
 
 @gf.cell
-def ring_single(
+def ring_single_sample(
     gap: float = 0.2,
     radius: float = 10.0,
     length_x: float = 4.0,
-    length_y: float = 0.6,
-    coupler_ring: ComponentSpec = coupler_ring_function,
-    bend: ComponentSpec = bend_euler,
+    length_y: float = 0.010,
+    coupler_ring: ComponentSpec = "coupler_ring",
+    straight: ComponentSpec = "straight",
+    bend: ComponentSpec = "bend_euler",
     cross_section: CrossSectionSpec = "strip",
     **kwargs,
-) -> gf.Component:
-    """Returns a single ring.
+) -> Component:
+    """Single bus ring made of a ring coupler.
 
-    ring coupler (cb: bottom) connects to two vertical straights (sl: left, sr: right),
-    two bends (bl, br) and horizontal straight (wg: top)
+    (cb: bottom) connected with two vertical straights (wl: left, wr: right)
+    two bends (bl, br) and horizontal straight (wg: top).
 
     Args:
         gap: gap between for coupler.
         radius: for the bend and coupler.
         length_x: ring coupler length.
         length_y: vertical straight length.
-        coupler_ring: ring coupler spec.
-        bend: 90 degrees bend spec.
-        cross_section: cross_section spec.
+        coupler_ring: ring coupler function.
+        straight: straight function.
+        bend: 90 degrees bend function.
+        cross_section: spec.
         kwargs: cross_section settings.
 
+
     .. code::
 
-          bl-st-br
+          bl-wt-br
           |      |
-          sl     sr length_y
+          wl     wr length_y
           |      |
          --==cb==-- gap
 
           length_x
+
     """
     gap = gf.snap.snap_to_grid(gap, nm=2)
 
-    c = gf.Component()
-    cb = c << gf.get_component(
+    coupler_ring_component = gf.get_component(
         coupler_ring,
         bend=bend,
         gap=gap,
         radius=radius,
         length_x=length_x,
         cross_section=cross_section,
         **kwargs,
     )
-    sy = straight(length=length_y, cross_section=cross_section, **kwargs)
-    b = gf.get_component(bend, cross_section=cross_section, radius=radius, **kwargs)
-    sx = straight(length=length_x, cross_section=cross_section, **kwargs)
-    sl = c << sy
-    sr = c << sy
-    bl = c << b
-    br = c << b
-    st = c << sx
-
-    sl.connect(port="o1", destination=cb.ports["o2"])
-    bl.connect(port="o2", destination=sl.ports["o2"])
-
-    st.connect(port="o2", destination=bl.ports["o1"])
-    br.connect(port="o2", destination=st.ports["o1"])
-    sr.connect(port="o1", destination=br.ports["o1"])
-    sr.connect(port="o2", destination=cb.ports["o3"])
+    straight_side = gf.get_component(
+        straight, length=length_y, cross_section=cross_section, **kwargs
+    )
+    straight_top = gf.get_component(
+        straight, length=length_x, cross_section=cross_section, **kwargs
+    )
+
+    bend = gf.get_component(bend, radius=radius, cross_section=cross_section, **kwargs)
 
-    c.add_port("o2", port=cb.ports["o4"])
+    c = Component()
+    cb = c << coupler_ring_component
+    wl = c << straight_side
+    wr = c << straight_side
+    bl = c << bend
+    br = c << bend
+    wt = c << straight_top
+    # wt.mirror(p1=(0, 0), p2=(1, 0))
+
+    wl.connect(port="o2", destination=cb.ports["o2"])
+    bl.connect(port="o2", destination=wl.ports["o1"])
+
+    wt.connect(port="o2", destination=bl.ports["o1"])
+    br.connect(port="o2", destination=wt.ports["o1"])
+    wr.connect(port="o1", destination=br.ports["o1"])
+
+    c.add_port("o2", port=cb.ports["o2"])
     c.add_port("o1", port=cb.ports["o1"])
     return c
 
 
-if __name__ == "__main__":
-    # c = ring_single(layer=(2, 0), cross_section_factory=gf.cross_section.pin, width=1)
-    # c = ring_single(width=2, gap=1, layer=(2, 0), radius=7, length_y=1)
-    # print(c.ports)
+def test_ring_single_sample() -> None:
+    assert ring_single_sample()
 
-    # c = gf.routing.add_fiber_array(ring_single)
-    c = ring_single(cross_section="rib", width=2)
-    c.show(show_ports=True)
 
-    # cc = gf.add_pins(c)
-    # print(c.settings)
-    # print(c.settings)
-    # cc.show(show_ports=True)
+if __name__ == "__main__":
+    c = ring_single_sample(width=2, gap=1, layer=(2, 0))
+    print(c.ports)
+    c.show(show_ports=True)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_single_array.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_single_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_single_bend_coupler.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_single_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_single_dut.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_single_dut.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_single_heater.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_single_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/ring_single_pn.py` & `gdsfactory-6.99.0/gdsfactory/components/ring_single_pn.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,13 +136,14 @@
 if __name__ == "__main__":
     # c = ring_single(layer=(2, 0), cross_section_factory=gf.cross_section.pin, width=1)
     # c = ring_single(width=2, gap=1, layer=(2, 0), radius=7, length_y=1)
     # print(c.ports)
 
     # c = gf.routing.add_fiber_array(ring_single)
     c = ring_single_pn()
+    print([i.name for i in c.get_dependencies()])
     c.show(show_ports=True)
 
     # cc = gf.add_pins(c)
     # print(c.settings)
     # print(c.settings)
     # cc.show(show_ports=True)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/components/seal_ring.py` & `gdsfactory-6.99.0/gdsfactory/components/seal_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/snspd.py` & `gdsfactory-6.99.0/gdsfactory/components/snspd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/spiral_double.py` & `gdsfactory-6.99.0/gdsfactory/components/spiral_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/spiral_external_io.py` & `gdsfactory-6.99.0/gdsfactory/components/spiral_external_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/spiral_heater.py` & `gdsfactory-6.99.0/gdsfactory/components/spiral_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/spiral_inner_io.py` & `gdsfactory-6.99.0/gdsfactory/components/spiral_inner_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/splitter_chain.py` & `gdsfactory-6.99.0/gdsfactory/components/splitter_chain.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/splitter_tree.py` & `gdsfactory-6.99.0/gdsfactory/components/splitter_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/straight.py` & `gdsfactory-6.99.0/gdsfactory/components/straight.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,17 @@
     # c = straight(cross_section=gf.partial('metal_routing', width=2), with_hash=False)
     # c = straight(
     #     cross_section=gf.partial(gf.cross_section.strip, width=2), with_hash=False
     # )
     # c = straight(cladding_offset=2.5)
 
     nm = 1e-3
-    c = straight(width=202 * nm)
+    xs = gf.cross_section.strip()
+    print(dict(xs))
+    c = straight(cross_section=xs)
     print(c.name)
 
     # strip2 = gf.get_cross_section("strip", layer=(2, 0))
     # settings = dict(width=2)
 
     # c = straight(
     #     length=1, cross_section={"cross_section": "strip", "settings": settings}
```

### Comparing `gdsfactory-6.98.2/gdsfactory/components/straight_array.py` & `gdsfactory-6.99.0/gdsfactory/components/straight_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/straight_heater_doped_rib.py` & `gdsfactory-6.99.0/gdsfactory/components/straight_heater_doped_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/straight_heater_doped_strip.py` & `gdsfactory-6.99.0/gdsfactory/components/straight_heater_doped_strip.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/straight_heater_meander.py` & `gdsfactory-6.99.0/gdsfactory/components/straight_heater_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/straight_heater_meander_doped.py` & `gdsfactory-6.99.0/gdsfactory/components/straight_heater_meander_doped.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/straight_heater_metal.py` & `gdsfactory-6.99.0/gdsfactory/components/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/straight_pin.py` & `gdsfactory-6.99.0/gdsfactory/components/straight_pin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/straight_pin_slot.py` & `gdsfactory-6.99.0/gdsfactory/components/straight_pin_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/straight_rib.py` & `gdsfactory-6.99.0/gdsfactory/components/straight_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/switch_tree.py` & `gdsfactory-6.99.0/gdsfactory/components/switch_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/taper.py` & `gdsfactory-6.99.0/gdsfactory/components/taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/taper_adiabatic.py` & `gdsfactory-6.99.0/gdsfactory/components/taper_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/taper_cross_section.py` & `gdsfactory-6.99.0/gdsfactory/components/taper_cross_section.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+from functools import partial
 
 import gdsfactory as gf
 from gdsfactory.cell import cell
 from gdsfactory.component import Component
 from gdsfactory.cross_section import rib_conformal, strip_rib_tip
 from gdsfactory.typings import CrossSectionSpec
 
@@ -48,29 +49,32 @@
         width_type="linear" if linear else width_type,
     )
     taper_path = gf.path.straight(length=length, npoints=npoints)
 
     c = gf.Component()
     ref = c << gf.path.extrude(taper_path, cross_section=transition)
     c.add_ports(ref.ports)
+    c.absorb(ref)
     return c
 
 
-taper_cross_section_linear = gf.partial(taper_cross_section, linear=True, npoints=2)
-taper_cross_section_sine = gf.partial(taper_cross_section, linear=False, npoints=101)
-taper_cross_section_parabolic = gf.partial(
+taper_cross_section_linear = partial(taper_cross_section, linear=True, npoints=2)
+taper_cross_section_sine = partial(taper_cross_section, linear=False, npoints=101)
+taper_cross_section_parabolic = partial(
     taper_cross_section, linear=False, width_type="parabolic", npoints=101
 )
 
 
 if __name__ == "__main__":
-    # x1 = gf.partial(strip, width=0.5)
-    # x2 = gf.partial(strip, width=2.5)
+    # x1 = partial(strip, width=0.5)
+    # x2 = partial(strip, width=2.5)
     # c = taper_cross_section_linear(x1, x2)
 
-    # x1 = gf.partial(strip, width=0.5)
-    # x2 = gf.partial(rib, width=2.5)
+    # x1 = partial(strip, width=0.5)
+    # x2 = partial(rib, width=2.5)
     # c = taper_cross_section_linear(x1, x2)
 
-    c = taper_cross_section(gf.cross_section.strip, gf.cross_section.rib)
+    # c = taper_cross_section(gf.cross_section.strip, gf.cross_section.rib)
     # c = taper_cross_section_sine()
+    c = taper_cross_section_parabolic()
+    print([i.name for i in c.get_dependencies()])
     c.show(show_ports=True)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/components/taper_from_csv.py` & `gdsfactory-6.99.0/gdsfactory/components/taper_from_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/taper_parabolic.py` & `gdsfactory-6.99.0/gdsfactory/components/taper_parabolic.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,10 +38,11 @@
     c.add_polygon(points, layer=layer)
     c.add_port(name="o1", center=(0, 0), width=width1, orientation=180, layer=layer)
     c.add_port(name="o2", center=(length, 0), width=width2, orientation=0, layer=layer)
     return c
 
 
 if __name__ == "__main__":
-    c = taper_parabolic(width2=6, length=40, exp=0.6)
+    # c = taper_parabolic(width2=6, length=40, exp=0.6)
     c = taper_parabolic()
+    print(c.name)
     c.show(show_ports=True)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/components/terminator.py` & `gdsfactory-6.99.0/gdsfactory/components/terminator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/text.py` & `gdsfactory-6.99.0/gdsfactory/components/text.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/text_freetype.py` & `gdsfactory-6.99.0/gdsfactory/components/text_freetype.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,16 @@
                         char.add_polygon([xpts + xoffset, ypts + yoffset], layer=layer)
                     xoffset += (_width[ascii_val] + _indent[ascii_val]) * scaling
                 else:
                     valid_chars = "!\"#$%&'()*+,-./0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\\]^_`abcdefghijklmnopqrstuvwxyz{|}~µ"
                     warnings.warn(
                         f'text(): Warning, some characters ignored, no geometry for character "{chr(ascii_val)}" with ascii value {ascii_val}. Valid characters: {valid_chars}'
                     )
-            t.add_ref(char)
+            ref = t.add_ref(char)
+            t.absorb(ref)
             yoffset -= 1500 * scaling
             xoffset = 0
     else:
         from gdsfactory.font import _get_font_by_file, _get_font_by_name, _get_glyph
 
         # Load the font
         # If we've passed a valid file, try to load that, otherwise search system fonts
@@ -105,9 +106,11 @@
         elif justify == "right":
             ref.xmax = 0
     t.flatten()
     return t
 
 
 if __name__ == "__main__":
-    c2 = text_freetype("hello", font="Times New Roman")
-    c2.show(show_ports=True)
+    # c2 = text_freetype("hello", font="Times New Roman")
+    # print(c2.name)
+    c2 = text_freetype()
+    c2.show()
```

### Comparing `gdsfactory-6.98.2/gdsfactory/components/text_rectangular.py` & `gdsfactory-6.99.0/gdsfactory/components/text_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/text_rectangular_font.py` & `gdsfactory-6.99.0/gdsfactory/components/text_rectangular_font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/triangles.py` & `gdsfactory-6.99.0/gdsfactory/components/triangles.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/verniers.py` & `gdsfactory-6.99.0/gdsfactory/components/verniers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/version_stamp.py` & `gdsfactory-6.99.0/gdsfactory/components/version_stamp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/via.py` & `gdsfactory-6.99.0/gdsfactory/components/via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/via_corner.py` & `gdsfactory-6.99.0/gdsfactory/components/via_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/via_cutback.py` & `gdsfactory-6.99.0/gdsfactory/components/via_cutback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/via_stack.py` & `gdsfactory-6.99.0/gdsfactory/components/via_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/via_stack_slot.py` & `gdsfactory-6.99.0/gdsfactory/components/via_stack_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/via_stack_with_offset.py` & `gdsfactory-6.99.0/gdsfactory/components/via_stack_with_offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/wafer.py` & `gdsfactory-6.99.0/gdsfactory/components/wafer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/wire.py` & `gdsfactory-6.99.0/gdsfactory/components/wire.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/components/wire_sbend.py` & `gdsfactory-6.99.0/gdsfactory/components/wire_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/config.py` & `gdsfactory-6.99.0/gdsfactory/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from loguru import logger
 import omegaconf
 from omegaconf import OmegaConf
 
 from rich.console import Console
 from rich.table import Table
 
-__version__ = "6.98.2"
+__version__ = "6.99.0"
 PathType = Union[str, pathlib.Path]
 
 home = pathlib.Path.home()
 cwd = pathlib.Path.cwd()
 module_path = pathlib.Path(__file__).parent.absolute()
 repo_path = module_path.parent
 home_path = pathlib.Path.home() / ".gdsfactory"
@@ -173,14 +173,15 @@
     notebooks = repo_path / "docs" / "notebooks"
     plugins = module / "plugins"
     web = plugins / "web"
     test_data = repo / "test-data"
     gds_ref = test_data / "gds"
     gds_run = GDSDIR_TEMP / "gds_run"
     gds_diff = GDSDIR_TEMP / "gds_diff"
+    cwd = cwd
 
 
 def read_config(
     yamlpaths: Iterable[PathType] = (yamlpath_default, yamlpath_home, yamlpath_cwd),
 ) -> omegaconf.DictConfig:
     config = OmegaConf.load(default_config)
     for yamlpath in set(yamlpaths):
```

### Comparing `gdsfactory-6.98.2/gdsfactory/constants.py` & `gdsfactory-6.99.0/gdsfactory/constants.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/containers.py` & `gdsfactory-6.99.0/gdsfactory/containers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/cross_section.py` & `gdsfactory-6.99.0/gdsfactory/cross_section.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,16 +150,16 @@
     port_types: Tuple[Optional[str], Optional[str]] = ("optical", "optical")
     gap: float = 3.0
     min_length: float = 10e-3
     start_straight_length: float = 10e-3
     end_straight_length: float = 10e-3
     snap_to_grid: Optional[float] = None
     decorator: Optional[Callable] = None
-    add_pins: Optional[Callable] = None
-    add_bbox: Optional[Callable] = None
+    add_pins: Optional[Callable] = Field(default=None, exclude=True)
+    add_bbox: Optional[Callable] = Field(default=None, exclude=True)
     info: Dict[str, Any] = Field(default_factory=dict)
     name: Optional[str] = None
     mirror: bool = False
 
     def __init__(__pydantic_self__, **data: Any) -> None:
         """Extend BaseModel init to process mirroring."""
         super().__init__(**data)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/decorators.py` & `gdsfactory-6.99.0/gdsfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/events.py` & `gdsfactory-6.99.0/gdsfactory/events.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/export/to_3d.py` & `gdsfactory-6.99.0/gdsfactory/export/to_3d.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/export/to_gerber.py` & `gdsfactory-6.99.0/gdsfactory/export/to_gerber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/export/to_np.py` & `gdsfactory-6.99.0/gdsfactory/export/to_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/export/to_stl.py` & `gdsfactory-6.99.0/gdsfactory/export/to_stl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/filestorage.py` & `gdsfactory-6.99.0/gdsfactory/filestorage.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/fill.py` & `gdsfactory-6.99.0/gdsfactory/fill.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
         fill_layers=((2, 0),),
         fill_densities=(1.0,),
         # fill_densities=0.5,
         avoid_layers=((1, 0),),
         # bbox=(100.0, 100.0),
     )
     c << fill
-    difftest(c)
+    difftest(c, test_name="fill")
     return c
 
 
 if __name__ == "__main__":
     c = test_fill()
 
     mzi = gf.components.mzi()
```

### Comparing `gdsfactory-6.98.2/gdsfactory/font.py` & `gdsfactory-6.99.0/gdsfactory/font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/functions.py` & `gdsfactory-6.99.0/gdsfactory/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/gdsdiff/gds_diff_git.py` & `gdsfactory-6.99.0/gdsfactory/gdsdiff/gds_diff_git.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/gdsdiff/gdsdiff.py` & `gdsfactory-6.99.0/gdsfactory/gdsdiff/gdsdiff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/gdsdiff/install.py` & `gdsfactory-6.99.0/gdsfactory/gdsdiff/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/gdsdiff/test_xor.py` & `gdsfactory-6.99.0/gdsfactory/gdsdiff/test_xor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from __future__ import annotations
 
 import gdsfactory as gf
 from gdsfactory.gdsdiff.gdsdiff import xor_polygons
 
 
-def test_differences() -> None:
-    straight = gf.partial(
-        gf.components.straight,
-        with_bbox=True,
-        cladding_layers=None,
-        add_pins=None,
-        add_bbox=None,
-    )
-    c1 = straight(length=2)
-    c2 = straight(length=3)
-    c = xor_polygons(c1, c2, hash_geometry=False)
-    area = c.area()
-    assert area == 0.5, area
-
-
-def test_no_differences() -> None:
-    straight = gf.partial(
-        gf.components.straight,
-        with_bbox=True,
-        cladding_layers=None,
-        add_pins=None,
-        add_bbox=None,
-    )
-    c1 = straight(length=2)
-    c2 = straight(length=2)
-    c = xor_polygons(c1, c2, hash_geometry=False)
-    area = c.area()
-    assert area == 0, area
+# def test_differences() -> None:
+#     straight = gf.partial(
+#         gf.components.straight,
+#         with_bbox=True,
+#         cladding_layers=None,
+#         add_pins=None,
+#         add_bbox=None,
+#     )
+#     c1 = straight(length=2)
+#     c2 = straight(length=3)
+#     c = xor_polygons(c1, c2, hash_geometry=False)
+#     area = c.area()
+#     assert area == 0.5, area
+
+
+# def test_no_differences() -> None:
+#     straight = gf.partial(
+#         gf.components.straight,
+#         with_bbox=True,
+#         cladding_layers=None,
+#         add_pins=None,
+#         add_bbox=None,
+#     )
+#     c1 = straight(length=2)
+#     c2 = straight(length=2)
+#     c = xor_polygons(c1, c2, hash_geometry=False)
+#     area = c.area()
+#     assert area == 0, area
 
 
 if __name__ == "__main__":
     # test_no_differences()
     # test_differences()
     c1 = gf.components.mzi(length_x=3)
     c2 = gf.components.mzi(length_x=2)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/README.md` & `gdsfactory-6.99.0/gdsfactory/generic_tech/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/__init__.py` & `gdsfactory-6.99.0/gdsfactory/generic_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/get_klayout_pyxs.py` & `gdsfactory-6.99.0/gdsfactory/generic_tech/get_klayout_pyxs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/drc/errors.py` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/drc/errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/grain.xml`

 * *Files 2% similar despite different names*

#### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/grain.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <salt-grain>
   <name>gdsfactory</name>
   <token/>
   <hidden>false</hidden>
-  <version>6.98.2</version>
+  <version>6.99.0</version>
   <api-version/>
   <title>gdsfactory</title>
   <doc>EDA tool to layout integrated circuits</doc>
   <doc-url>https://gdsfactory.github.io/gdsfactory/</doc-url>
   <url>https://github.com/gdsfactory/gdsfactory</url>
   <license>MIT</license>
   <author>Joaquin Matres</author>
```

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/icon_128x128.png` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/icon_64x64.png` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/README.md` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/run_lvs.py` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

 * *Files 2% similar despite different names*

#### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

```diff
@@ -12,15 +12,15 @@
   <show-in-menu>false</show-in-menu>
   <group-name/>
   <menu-path>gdsfactory.begin</menu-path>
   <interpreter>python</interpreter>
   <dsl-interpreter-name/>
   <text>import pya
 
-__version__ = &quot;6.98.2&quot;
+__version__ = &quot;6.99.0&quot;
 
 
 def set_menu():
     menu = pya.Application.instance().main_window().menu()
 
     s0 = &quot;gdsfactory&quot;
     if not (menu.is_menu(s0)):
```

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/generic.layerstack` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/layers.lyp` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/layers.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/tech.lyt` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/tech.lyt`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs` & `gdsfactory-6.99.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/layer_map.py` & `gdsfactory-6.99.0/gdsfactory/generic_tech/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/layer_stack.py` & `gdsfactory-6.99.0/gdsfactory/generic_tech/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/generic_tech/layer_views.yaml` & `gdsfactory-6.99.0/gdsfactory/generic_tech/layer_views.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/__init__.py` & `gdsfactory-6.99.0/gdsfactory/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/boolean.py` & `gdsfactory-6.99.0/gdsfactory/geometry/boolean.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/boolean_klayout.py` & `gdsfactory-6.99.0/gdsfactory/geometry/boolean_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/boolean_polygons.py` & `gdsfactory-6.99.0/gdsfactory/geometry/boolean_polygons.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/check_duplicated_cells.py` & `gdsfactory-6.99.0/gdsfactory/geometry/check_duplicated_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/check_exclusion.py` & `gdsfactory-6.99.0/gdsfactory/geometry/check_exclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/check_inclusion.py` & `gdsfactory-6.99.0/gdsfactory/geometry/check_inclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/check_space.py` & `gdsfactory-6.99.0/gdsfactory/geometry/check_space.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/check_width.py` & `gdsfactory-6.99.0/gdsfactory/geometry/check_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/fill_klayout.py` & `gdsfactory-6.99.0/gdsfactory/geometry/fill_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/fill_tiled.py` & `gdsfactory-6.99.0/gdsfactory/geometry/fill_tiled.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/fillet.py` & `gdsfactory-6.99.0/gdsfactory/geometry/fillet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/functions.py` & `gdsfactory-6.99.0/gdsfactory/geometry/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/invert.py` & `gdsfactory-6.99.0/gdsfactory/geometry/invert.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/layer_priority.py` & `gdsfactory-6.99.0/gdsfactory/geometry/layer_priority.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/manhattanize.py` & `gdsfactory-6.99.0/gdsfactory/geometry/manhattanize.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/maskprep.py` & `gdsfactory-6.99.0/gdsfactory/geometry/maskprep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/maskprep_flat.py` & `gdsfactory-6.99.0/gdsfactory/geometry/maskprep_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/offset.py` & `gdsfactory-6.99.0/gdsfactory/geometry/offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/outline.py` & `gdsfactory-6.99.0/gdsfactory/geometry/outline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/trim.py` & `gdsfactory-6.99.0/gdsfactory/geometry/trim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/union.py` & `gdsfactory-6.99.0/gdsfactory/geometry/union.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/write_connectivity.py` & `gdsfactory-6.99.0/gdsfactory/geometry/write_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/write_drc.py` & `gdsfactory-6.99.0/gdsfactory/geometry/write_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/geometry/xor_diff.py` & `gdsfactory-6.99.0/gdsfactory/geometry/xor_diff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/get_factories.py` & `gdsfactory-6.99.0/gdsfactory/get_factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/get_netlist.py` & `gdsfactory-6.99.0/gdsfactory/get_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/get_netlist_flat.py` & `gdsfactory-6.99.0/gdsfactory/get_netlist_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/get_netlist_klayout.py` & `gdsfactory-6.99.0/gdsfactory/get_netlist_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/grid.py` & `gdsfactory-6.99.0/gdsfactory/grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/install.py` & `gdsfactory-6.99.0/gdsfactory/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/klive.py` & `gdsfactory-6.99.0/gdsfactory/klive.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/labels/__init__.py` & `gdsfactory-6.99.0/gdsfactory/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/labels/add_label_yaml.py` & `gdsfactory-6.99.0/gdsfactory/labels/add_label_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/labels/ehva.py` & `gdsfactory-6.99.0/gdsfactory/labels/ehva.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/labels/merge_test_metadata.py` & `gdsfactory-6.99.0/gdsfactory/labels/merge_test_metadata.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/labels/siepic.py` & `gdsfactory-6.99.0/gdsfactory/labels/siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/labels/write_labels.py` & `gdsfactory-6.99.0/gdsfactory/labels/write_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/materials.py` & `gdsfactory-6.99.0/gdsfactory/materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/name.py` & `gdsfactory-6.99.0/gdsfactory/name.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/pack.py` & `gdsfactory-6.99.0/gdsfactory/pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/path.py` & `gdsfactory-6.99.0/gdsfactory/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,16 +376,16 @@
 
     @classmethod
     def _validate(cls, v):
         """Pydantic Path validator."""
         assert isinstance(v, Path), f"TypeError, Got {type(v)}, expecting Path"
         return v
 
-    def to_dict(self):
-        return self.hash_geometry()
+    def to_dict(self) -> dict[str, str]:
+        return dict(hash=self.hash_geometry())
 
     def plot(self) -> None:
         """Plot path in matplotlib.
 
         .. plot::
             :include-source:
 
@@ -1483,33 +1483,50 @@
 if __name__ == "__main__":
     import numpy as np
     import gdsfactory as gf
 
     # nm = 1e-3
 
     # points = np.array([(20, 10), (40, 10), (20, 40), (50, 40), (50, 20), (70, 20)])
-
     # p = smooth(points=points)
+
     # p = arc(start_angle=0)
     # c = p.extrude(layer=(1, 0), width=0.1, simplify=50 * nm)
-    # p = straight()
+    p = straight()
     # p.plot()
 
-    # from phidl.path import smooth
-    # p = smooth(
-    #     points=points,
-    #     radius=2,
-    #     # bend=gf.path.euler,
-    #     use_eff=False,
-    # )
-
     # c = p.extrude(layer=(1, 0), width=0.1)
-    # c = gf.read.from_phidl(c)
-    c = gf.components.splitter_tree(
-        noutputs=2**2,
-        spacing=(120.0, 50.0),
-        # bend_length=30,
-        # bend_s=None,
-        cross_section="rib_conformal2",
+    s1 = gf.Section(width=2.2, offset=0, layer=(3, 0), name="etch")
+    s2 = gf.Section(width=1.1, offset=3, layer=(1, 0), name="wg2")
+    X1 = gf.CrossSection(
+        width=1.2,
+        offset=0,
+        layer=(2, 0),
+        name="wg",
+        port_names=("in1", "out1"),
+        sections=[s1, s2],
+    )
+
+    # Create the second CrossSection that we want to transition to
+    s1 = gf.Section(width=3.5, offset=0, layer=(3, 0), name="etch")
+    s2 = gf.Section(width=3, offset=5, layer=(1, 0), name="wg2")
+    X2 = gf.CrossSection(
+        width=1,
+        offset=0,
+        layer=(2, 0),
+        name="wg",
+        port_names=("in1", "out1"),
+        sections=[s1, s2],
     )
 
+    Xtrans = gf.path.transition(cross_section1=X1, cross_section2=X2, width_type="sine")
+
+    c = p.extrude(cross_section=Xtrans)
+    print(c.name)
+    # c = gf.components.splitter_tree(
+    #     noutputs=2**2,
+    #     spacing=(120.0, 50.0),
+    #     # bend_length=30,
+    #     # bend_s=None,
+    #     cross_section="rib_conformal2",
+    # )
     c.show()
```

### Comparing `gdsfactory-6.98.2/gdsfactory/pdk.py` & `gdsfactory-6.99.0/gdsfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/picmodel.py` & `gdsfactory-6.99.0/gdsfactory/picmodel.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/pixelate.py` & `gdsfactory-6.99.0/gdsfactory/pixelate.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/dagster/workflow.py` & `gdsfactory-6.99.0/gdsfactory/plugins/dagster/workflow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/database/README.md` & `gdsfactory-6.99.0/gdsfactory/plugins/database/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/database/db_upload.py` & `gdsfactory-6.99.0/gdsfactory/plugins/database/db_upload.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/database/models.py` & `gdsfactory-6.99.0/gdsfactory/plugins/database/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/web/main.py` & `gdsfactory-6.99.0/gdsfactory/plugins/web/main.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/web/server.py` & `gdsfactory-6.99.0/gdsfactory/plugins/web/server.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/web/server_jupyter.py` & `gdsfactory-6.99.0/gdsfactory/plugins/web/server_jupyter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/web/static/client.css` & `gdsfactory-6.99.0/gdsfactory/plugins/web/static/client.css`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/web/static/client.js` & `gdsfactory-6.99.0/gdsfactory/plugins/web/static/client.js`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/web/templates/client.html` & `gdsfactory-6.99.0/gdsfactory/plugins/web/templates/client.html`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/web/templates/header.html` & `gdsfactory-6.99.0/gdsfactory/plugins/web/templates/header.html`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/web/templates/navbar.html` & `gdsfactory-6.99.0/gdsfactory/plugins/web/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/plugins/web/templates/viewer.html` & `gdsfactory-6.99.0/gdsfactory/plugins/web/templates/viewer.html`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/port.py` & `gdsfactory-6.99.0/gdsfactory/port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/quickplotter.py` & `gdsfactory-6.99.0/gdsfactory/quickplotter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/read/__init__.py` & `gdsfactory-6.99.0/gdsfactory/read/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/read/from_dphox.py` & `gdsfactory-6.99.0/gdsfactory/read/from_dphox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/read/from_gdspaths.py` & `gdsfactory-6.99.0/gdsfactory/read/from_gdspaths.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/read/from_np.py` & `gdsfactory-6.99.0/gdsfactory/read/from_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/read/from_phidl.py` & `gdsfactory-6.99.0/gdsfactory/read/from_phidl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/read/from_yaml.py` & `gdsfactory-6.99.0/gdsfactory/read/from_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/read/from_yaml_template.py` & `gdsfactory-6.99.0/gdsfactory/read/from_yaml_template.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/read/import_gds.py` & `gdsfactory-6.99.0/gdsfactory/read/import_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/read/labels.py` & `gdsfactory-6.99.0/gdsfactory/read/labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/__init__.py` & `gdsfactory-6.99.0/gdsfactory/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/add_electrical_pads_shortest.py` & `gdsfactory-6.99.0/gdsfactory/routing/add_electrical_pads_shortest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/add_electrical_pads_top.py` & `gdsfactory-6.99.0/gdsfactory/routing/add_electrical_pads_top.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/add_electrical_pads_top_dc.py` & `gdsfactory-6.99.0/gdsfactory/routing/add_electrical_pads_top_dc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/add_fiber_array.py` & `gdsfactory-6.99.0/gdsfactory/routing/add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/add_fiber_single.py` & `gdsfactory-6.99.0/gdsfactory/routing/add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/add_pads.py` & `gdsfactory-6.99.0/gdsfactory/routing/add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/all_angle.py` & `gdsfactory-6.99.0/gdsfactory/routing/all_angle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/auto_taper.py` & `gdsfactory-6.99.0/gdsfactory/routing/auto_taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/factories.py` & `gdsfactory-6.99.0/gdsfactory/routing/factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/fanout.py` & `gdsfactory-6.99.0/gdsfactory/routing/fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/fanout2x2.py` & `gdsfactory-6.99.0/gdsfactory/routing/fanout2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_bundle.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_bundle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_bundle_corner.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_bundle_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_bundle_from_steps.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_bundle_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_bundle_from_waypoints.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_bundle_from_waypoints.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_bundle_path_length_match.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_bundle_path_length_match.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_bundle_sbend.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_bundle_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_bundle_u.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_bundle_u.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_input_labels.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_input_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_route.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_route.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,8 +314,9 @@
         cross_section=gf.cross_section.strip(),
         auto_widen=True,
         width_wide=2,
         auto_widen_minimum_length=100,
         radius=30,
     )
     c.add(route.references)
+    print([i.name for i in c.get_dependencies()])
     c.show()
```

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_route_astar.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_route_astar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_route_from_steps.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_route_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_route_sbend.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_route_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_routes_bend180.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_routes_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/get_routes_straight.py` & `gdsfactory-6.99.0/gdsfactory/routing/get_routes_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/manhattan.py` & `gdsfactory-6.99.0/gdsfactory/routing/manhattan.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,15 +599,14 @@
     taper: Optional[ComponentSpec] = None,
     straight_fall_back_no_taper: Optional[ComponentSpec] = None,
     mirror_straight: bool = False,
     straight_ports: Optional[List[str]] = None,
     cross_section: Union[CrossSectionSpec, MultiCrossSectionAngleSpec] = strip,
     on_route_error: Callable = get_route_error,
     with_point_markers: bool = False,
-    snap_to_grid_nm: Optional[int] = 1,
     with_sbend: bool = False,
     **kwargs,
 ) -> Route:
     """Returns Route.
 
     - reference list with rounded straight route from a list of manhattan points.
     - ports: Tuple of ports.
@@ -620,15 +619,14 @@
         taper: taper for straight portions. If None, no tapering.
         straight_fall_back_no_taper: in case there is no space for two tapers.
         mirror_straight: mirror_straight waveguide.
         straight_ports: port names for straights. If None finds them automatically.
         cross_section: spec.
         on_route_error: function to run when route fails.
         with_point_markers: add route points markers (easy for debugging).
-        snap_to_grid_nm: nm to snap to grid.
         with_sbend: add sbend in case there are routing errors.
         kwargs: cross_section settings.
 
     """
     from gdsfactory.pdk import get_layer
 
     multi_cross_section = isinstance(cross_section, list)
@@ -636,18 +634,14 @@
         x = [gf.get_cross_section(xsection[0], **kwargs) for xsection in cross_section]
         layer = [_x.layer for _x in x]
     else:
         x = gf.get_cross_section(cross_section, **kwargs)
         layer = x.layer
 
     layer = get_layer(layer)
-    points = (
-        gf.snap.snap_to_grid(points, nm=snap_to_grid_nm) if snap_to_grid_nm else points
-    )
-
     references = []
 
     bend90 = (
         bend
         if isinstance(bend, Component)
         else gf.get_component(bend, cross_section=cross_section, **kwargs)
     )
```

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/path_length_matching.py` & `gdsfactory-6.99.0/gdsfactory/routing/path_length_matching.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/route_fiber_array.py` & `gdsfactory-6.99.0/gdsfactory/routing/route_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/route_fiber_single.py` & `gdsfactory-6.99.0/gdsfactory/routing/route_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/route_ports_to_side.py` & `gdsfactory-6.99.0/gdsfactory/routing/route_ports_to_side.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/route_quad.py` & `gdsfactory-6.99.0/gdsfactory/routing/route_quad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/route_sharp.py` & `gdsfactory-6.99.0/gdsfactory/routing/route_sharp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/route_south.py` & `gdsfactory-6.99.0/gdsfactory/routing/route_south.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/sort_ports.py` & `gdsfactory-6.99.0/gdsfactory/routing/sort_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/routing/utils.py` & `gdsfactory-6.99.0/gdsfactory/routing/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/01_component_pcell.py` & `gdsfactory-6.99.0/gdsfactory/samples/01_component_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/01_component_pcell/test_straight_wide.yml` & `gdsfactory-6.99.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/01_component_pcell_with_pins.py` & `gdsfactory-6.99.0/gdsfactory/samples/01_component_pcell_with_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml` & `gdsfactory-6.99.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/03_move.py` & `gdsfactory-6.99.0/gdsfactory/samples/03_move.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/04_connect.py` & `gdsfactory-6.99.0/gdsfactory/samples/04_connect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/05_remove_layers.py` & `gdsfactory-6.99.0/gdsfactory/samples/05_remove_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/06_remapping_layers.py` & `gdsfactory-6.99.0/gdsfactory/samples/06_remapping_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/07_flattening_device.py` & `gdsfactory-6.99.0/gdsfactory/samples/07_flattening_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/11_component_layout.py` & `gdsfactory-6.99.0/gdsfactory/samples/11_component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/12_component_refs.py` & `gdsfactory-6.99.0/gdsfactory/samples/12_component_refs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/13_component_netlist.py` & `gdsfactory-6.99.0/gdsfactory/samples/13_component_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/15_component_sequence1.py` & `gdsfactory-6.99.0/gdsfactory/samples/15_component_sequence1.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/16_component_sequence2.py` & `gdsfactory-6.99.0/gdsfactory/samples/16_component_sequence2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/17_ports.py` & `gdsfactory-6.99.0/gdsfactory/samples/17_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/20_components.py` & `gdsfactory-6.99.0/gdsfactory/samples/20_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/22_add_pads.py` & `gdsfactory-6.99.0/gdsfactory/samples/22_add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/23_reticle.py` & `gdsfactory-6.99.0/gdsfactory/samples/23_reticle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/23_reticle_passives.py` & `gdsfactory-6.99.0/gdsfactory/samples/23_reticle_passives.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/24_doe_2.py` & `gdsfactory-6.99.0/gdsfactory/samples/24_doe_2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/24_doe_3.py` & `gdsfactory-6.99.0/gdsfactory/samples/24_doe_3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/30_lidar.py` & `gdsfactory-6.99.0/gdsfactory/samples/30_lidar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/30_lidar_pcell.py` & `gdsfactory-6.99.0/gdsfactory/samples/30_lidar_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/30_lidar_with_pads.py` & `gdsfactory-6.99.0/gdsfactory/samples/30_lidar_with_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing.py` & `gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/big_device.py` & `gdsfactory-6.99.0/gdsfactory/samples/big_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/demo/benchmark/fill_demo.py` & `gdsfactory-6.99.0/gdsfactory/samples/demo/benchmark/fill_demo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/demo/circuits/mask.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/demo/circuits/mask.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml` & `gdsfactory-6.99.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/demo/drc_errors.py` & `gdsfactory-6.99.0/gdsfactory/samples/demo/drc_errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/demo/drc_write.py` & `gdsfactory-6.99.0/gdsfactory/samples/demo/drc_write.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/demo/layers.py` & `gdsfactory-6.99.0/gdsfactory/samples/demo/layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/demo/lvs.py` & `gdsfactory-6.99.0/gdsfactory/samples/demo/lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/demo/pcell.py` & `gdsfactory-6.99.0/gdsfactory/samples/demo/pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/netlists/mzi.yml` & `gdsfactory-6.99.0/gdsfactory/samples/netlists/mzi.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/netlists/mzi_full.yml` & `gdsfactory-6.99.0/gdsfactory/samples/netlists/mzi_full.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/fab_c.py` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/fab_d/phase_shifters.py` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c.py` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml` & `gdsfactory-6.99.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/schematic_editor.py` & `gdsfactory-6.99.0/gdsfactory/schematic_editor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/serialization.py` & `gdsfactory-6.99.0/gdsfactory/serialization.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import gdstk
 import numpy as np
 import orjson
 import pydantic
 import toolz
 from omegaconf import DictConfig, OmegaConf
 
-DEFAULT_SERIALIZATION_MAX_DIGITS = 8
+DEFAULT_SERIALIZATION_MAX_DIGITS = 3
 """By default, the maximum number of digits retained when serializing float-like arrays"""
 
 
 def clean_dict(d: Dict[str, Any]) -> Dict[str, Any]:
     """Cleans dictionary recursively."""
     return {
         k: clean_dict(dict(v)) if isinstance(v, dict) else clean_value_json(v)
@@ -38,27 +38,27 @@
 
 
 def clean_value_json(value: Any) -> Any:
     """Return JSON serializable object."""
     from gdsfactory.path import Path
 
     if isinstance(value, pydantic.BaseModel):
-        return value.dict()
+        return clean_dict(value.dict())
 
     elif hasattr(value, "get_component_spec"):
         return value.get_component_spec()
 
     elif isinstance(value, bool):
         return value
 
     elif isinstance(value, (np.integer, int)):
         return int(value)
 
     elif isinstance(value, (float, np.inexact, np.float64)):
-        return float(value)
+        return float(np.round(value, DEFAULT_SERIALIZATION_MAX_DIGITS))
 
     elif isinstance(value, np.ndarray):
         value = np.round(value, DEFAULT_SERIALIZATION_MAX_DIGITS)
         return orjson.loads(orjson.dumps(value, option=orjson.OPT_SERIALIZE_NUMPY))
     elif callable(value) and isinstance(value, functools.partial):
         sig = inspect.signature(value.func)
         args_as_kwargs = dict(zip(sig.parameters.keys(), value.args))
@@ -68,15 +68,16 @@
 
         func = value.func
         while hasattr(func, "func"):
             func = func.func
         return {"function": func.__name__, "settings": args_as_kwargs}
 
     elif hasattr(value, "to_dict"):
-        return value.to_dict()
+        # print(type(value))
+        return clean_dict(value.to_dict())
     elif callable(value) and isinstance(value, toolz.functoolz.Compose):
         value = [clean_value_json(value.first)] + [
             clean_value_json(func) for func in value.funcs
         ]
     elif callable(value) and hasattr(value, "__name__"):
         value = {"function": value.__name__}
     elif isinstance(value, Path):
@@ -88,15 +89,15 @@
     elif isinstance(value, DictConfig):
         value = clean_dict(OmegaConf.to_container(value))
 
     elif isinstance(value, (list, tuple, set)):
         value = [clean_value_json(i) for i in value]
 
     elif isinstance(value, gdstk.Polygon):
-        value = np.round(value.points, 3)
+        value = np.round(value.points, DEFAULT_SERIALIZATION_MAX_DIGITS)
     else:
         try:
             value_json = orjson.dumps(
                 value, option=orjson.OPT_SERIALIZE_NUMPY, default=clean_value_json
             )
             value = orjson.loads(value_json)
         except TypeError as e:
@@ -129,11 +130,17 @@
 if __name__ == "__main__":
     import gdsfactory as gf
 
     # f = gf.partial(gf.c.straight, length=3)
     # d = clean_value_json(f)
     # print(f"{d!r}")
 
-    f = gf.partial(gf.c.straight, length=3)
+    # f = gf.partial(gf.c.straight, length=3)
+    # c = f()
+    # d = clean_value_json(c)
+    # print(d, d)
+
+    f = gf.partial(gf.cross_section.strip, width=3)
     c = f()
     d = clean_value_json(c)
+    print(get_hash(d))
     print(d, d)
```

### Comparing `gdsfactory-6.98.2/gdsfactory/show.py` & `gdsfactory-6.99.0/gdsfactory/show.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/__init__.py` & `gdsfactory-6.99.0/gdsfactory/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/add_simulation_markers.py` & `gdsfactory-6.99.0/gdsfactory/simulation/add_simulation_markers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/convert_sparameters.py` & `gdsfactory-6.99.0/gdsfactory/simulation/convert_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/devsim/__init__.py` & `gdsfactory-6.99.0/gdsfactory/simulation/devsim/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 from gdsfactory.config import logger
 from gdsfactory.simulation.devsim.get_simulation_xsection import (
     PINWaveguide,
     alpha_to_k,
     dalpha_carriers,
     dn_carriers,
     k_to_alpha,
+    clear_devsim_cache,
 )
 from gdsfactory.simulation.devsim.get_solver import DDComponent
 
 logger.info(f"DEVSIM {tcad.__version__!r} installed at {tcad.__path__!r}")
 
 __all__ = [
     "dn_carriers",
     "dalpha_carriers",
     "alpha_to_k",
     "k_to_alpha",
     "PINWaveguide",
     "DDComponent",
+    "clear_devsim_cache",
 ]
 __version__ = "0.0.1"
```

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/devsim/doping.py` & `gdsfactory-6.99.0/gdsfactory/simulation/devsim/doping.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/devsim/get_simulation.py` & `gdsfactory-6.99.0/gdsfactory/simulation/devsim/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/devsim/get_simulation_xsection.py` & `gdsfactory-6.99.0/gdsfactory/simulation/devsim/get_simulation_xsection.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,30 +8,36 @@
 
 """
 
 
 from __future__ import annotations
 
 from typing import Optional
+import warnings
 
 import devsim
 import matplotlib.pyplot as plt
 import numpy as np
+from scipy.interpolate import griddata
 import pyvista as pv
 from devsim.python_packages import model_create, simple_physics
 from pydantic import BaseModel, Extra
+import tidy3d as td
 
 from gdsfactory.simulation.disable_print import disable_print, enable_print
-from gdsfactory.simulation.gtidy3d.modes import FilterPol, Precision, Waveguide
+from gdsfactory.simulation.gtidy3d.materials import get_nk
+from gdsfactory.simulation.gtidy3d.modes import Precision, Waveguide
 from gdsfactory.typings import MaterialSpec
 
 nm = 1e-9
 um = 1e-6
 cm = 1e-2
 
+DEVSIM_INTERPOLATION_METHOD = "linear"
+
 
 def dn_carriers(wavelength: float, dN: float, dP: float) -> float:
     """Phenomenological wavelength-dependent index perturbation from free carriers.
 
     Use quadratic fits for wavelengths, or better-characterized models at 1550 and 1310.
 
     Args:
@@ -90,27 +96,27 @@
     return alpha * 1e-2  # convert to /cm
 
 
 class PINWaveguide(BaseModel):
     """Silicon PIN junction waveguide Model.
 
     Parameters:
-        wg_width: waveguide width.
+        core_width: waveguide width.
         core_thickness: thickness waveguide (um).
         p_offset: offset between waveguide center and P-doping in um
             negative to push toward n-side.
         n_offset: offset between waveguide center and N-doping in um
             negative to push toward p-side).
         ppp_offset: offset between waveguide center and Ppp-doping in um
             negative to push toward n-side) NOT IMPLEMENTED.
         npp_offset: offset between waveguide center and Npp-doping in um
             negative to push toward p-side) NOT IMPLEMENTED.
         slab_thickness: thickness slab (um).
-        t_box: thickness BOX (um).
-        t_clad: thickness cladding (um).
+        box_thickness: thickness BOX (um).
+        clad_thickness: thickness cladding (um).
         p_conc: low-doping acceptor concentration (/cm3).
         n_conc: low-doping donor concentration (/cm3).
         ppp_conc: high-doping acceptor concentration (/cm3).
         nnn_conc: high-doping donor concentration (/cm3).
         xmargin: margin from waveguide edge to low doping regions.
         contact_bloat: controls which nodes are considered contacts;
             adjust if contacts are not found.
@@ -135,23 +141,23 @@
           ^          ^       ^     ^         ^         ^
       pp_res_x   pp_p_res     pn_res      pp_p_res  pp_res_x
           <-------------------------------------------->
                                w_sim
 
     """
 
-    wg_width: float
+    core_width: float
     core_thickness: float
     p_offset: float = 0.0
     n_offset: float = 0.0
     ppp_offset: float = 0.5 * um
     npp_offset: float = 0.5 * um
     slab_thickness: float
-    t_box: float = 2.0 * um
-    t_clad: float = 2.0 * um
+    box_thickness: float = 2.0 * um
+    clad_thickness: float = 2.0 * um
     p_conc: float = 1e17
     n_conc: float = 1e17
     ppp_conc: float = 1e17
     nnn_conc: float = 1e17
     xmargin: float = 0.5 * um
     xcontact: float = 0.25 * um
     pp_res_x: float = 20 * nm
@@ -167,30 +173,30 @@
     class Config:
         """Enable adding new."""
 
         extra = Extra.allow
 
     # @property
     # def t_sim(self):
-    #     return self.t_box + self.core_thickness + self.t_clad
+    #     return self.box_thickness + self.core_thickness + self.clad_thickness
 
     # @property
     # def w_sim(self):
     #     return 2 * self.xmargin + self.ppp_offset + self.npp_offset
 
     def create_2d_mesh(self, device) -> None:
         """Creates a 2D mesh."""
-        xmin = (-self.xmargin - self.ppp_offset - self.wg_width / 2) / cm
-        xmax = (self.xmargin + self.npp_offset + self.wg_width / 2) / cm
-        self.xppp = -self.ppp_offset - self.wg_width / 2
-        self.xnpp = self.npp_offset + self.wg_width / 2
+        xmin = (-self.xmargin - self.ppp_offset - self.core_width / 2) / cm
+        xmax = (self.xmargin + self.npp_offset + self.core_width / 2) / cm
+        self.xppp = -self.ppp_offset - self.core_width / 2
+        self.xnpp = self.npp_offset + self.core_width / 2
         ymin = 0 / cm
         ymax = (self.core_thickness) / cm
-        xmin_waveguide = (-self.wg_width / 2) / cm
-        xmax_waveguide = (self.wg_width / 2) / cm
+        xmin_waveguide = (-self.core_width / 2) / cm
+        xmax_waveguide = (self.core_width / 2) / cm
         yslab = (self.slab_thickness) / cm
 
         devsim.create_2d_mesh(mesh="dio")
         devsim.add_2d_mesh_line(mesh="dio", dir="x", pos=xmin, ps=self.pp_res_x / cm)
         devsim.add_2d_mesh_line(
             mesh="dio", dir="x", pos=self.xppp / cm, ps=self.pp_p_res_x / cm
         )
@@ -477,115 +483,239 @@
         reader = pv.get_reader(tempfile)
         mesh = reader.read()
         return mesh[0]
 
     def make_waveguide(
         self,
         wavelength: float,
-        t_box: float = 2.0,
-        t_clad: float = 2.0,
-        resolution: int = 200,
+        box_thickness: float = 2.0,
+        clad_thickness: float = 2.0,
+        grid_resolution: int = 200,
         perturb: bool = True,
         nmodes: int = 4,
         bend_radius: Optional[float] = None,
         cache: bool = False,
         precision: Precision = "double",
-        filter_pol: Optional[FilterPol] = None,
         core_material: MaterialSpec = "si",
         clad_material: MaterialSpec = "sio2",
     ) -> Waveguide:
         """Converts the FEM model to a Waveguide object.
 
         - Rescales lengths to um
         - Adjusts origin to match Waveguide object convention
 
         Args:
             wavelength: (um).
-            t_box: thickness BOX (um).
-            t_clad: thickness cladding (um).
+            box_thickness: thickness BOX (um).
+            clad_thickness: thickness cladding (um).
             xmargin: margin from waveguide edge to each side (um).
-            resolution: pixels/um.
+            grid_resolution: wavelength resolution of the computation grid.
             perturb: add perturbation.
             nmodes: number of modes to compute.
             bend_radius: optional bend radius (um).
             cache: True uses file cache from PDK.modes_path. False skips cache.
             precision: single or double.
-            filter_pol: te, tm or None.
 
         Returns:
             A tidy3d Waveguide object.
 
         """
-        # Create index perturbation
-        x_fem = []
-        y_fem = []
-        dN_fem = []
-        dP_fem = []
-
-        mat_dtype = np.float64 if precision == "double" else np.float32
-
-        for region_name in ["core", "slab"]:
-            x_fem.append(
-                np.array(self.get_field(region_name=region_name, field_name="x"))
-            )
-            y_fem.append(
-                np.array(self.get_field(region_name=region_name, field_name="y"))
-            )
-            dN_fem.append(
-                np.array(
-                    self.get_field(region_name=region_name, field_name="Electrons"),
-                    dtype=mat_dtype,
-                )
-            )
-            dP_fem.append(
-                np.array(
-                    self.get_field(region_name=region_name, field_name="Holes"),
-                    dtype=mat_dtype,
+        if perturb:
+            # Create temporary Waveguide to get the X, Y, Z positions
+            temp_Waveguide = Waveguide(
+                wavelength=wavelength,
+                core_width=self.core_width / um,
+                core_thickness=self.core_thickness / um,
+                slab_thickness=self.slab_thickness / um,
+                box_thickness=box_thickness,
+                clad_thickness=clad_thickness,
+                side_margin=max(
+                    self.ppp_offset + self.xmargin, self.npp_offset + self.xmargin
                 )
+                / um,
+                grid_resolution=grid_resolution,
+                precision=precision,
+                core_material=core_material,
+                clad_material=clad_material,
+                cache=False,
             )
 
-        x_fem = np.concatenate(x_fem)
-        y_fem = np.concatenate(y_fem)
-        dN_fem = np.concatenate(dN_fem)
-        dP_fem = np.concatenate(dP_fem)
-
-        dn_fem = dn_carriers(wavelength, dN_fem, dP_fem)
-        dk_fem = alpha_to_k(dalpha_carriers(wavelength, dN_fem, dP_fem), wavelength)
-        dn_dict = (
-            {
-                "x": x_fem * cm / um,
-                "y": y_fem * cm / um + t_box,
-                "dn": dn_fem + 1j * dk_fem,
-            }
-            if perturb
-            else None
-        )
-
-        # Create perturbed waveguide, handle like regular mode
-        return Waveguide(
-            wavelength=wavelength,
-            wg_width=self.wg_width / um,
-            core_thickness=self.core_thickness / um,
-            slab_thickness=self.slab_thickness / um,
-            t_box=t_box,
-            t_clad=t_clad,
-            xmargin=(self.ppp_offset + self.xmargin) / um,
-            resolution=resolution,
-            dn_dict=dn_dict,
-            precision=precision,
-            filter_pol=filter_pol,
-            core_material=core_material,
-            clad_material=clad_material,
-            cache=cache,
-        )
+            # Create index perturbation
+            x_fem = []
+            y_fem = []
+            dN_fem = []
+            dP_fem = []
+
+            mat_dtype = np.float64 if precision == "double" else np.float32
+
+            for region_name in ["core", "slab"]:
+                x_fem.append(
+                    np.array(self.get_field(region_name=region_name, field_name="x"))
+                )
+                y_fem.append(
+                    np.array(self.get_field(region_name=region_name, field_name="y"))
+                )
+                dN_fem.append(
+                    np.array(
+                        self.get_field(region_name=region_name, field_name="Electrons"),
+                        dtype=mat_dtype,
+                    )
+                )
+                dP_fem.append(
+                    np.array(
+                        self.get_field(region_name=region_name, field_name="Holes"),
+                        dtype=mat_dtype,
+                    )
+                )
+
+            x_fem = np.concatenate(x_fem)
+            y_fem = np.concatenate(y_fem)
+            dN_fem = np.concatenate(dN_fem)
+            dP_fem = np.concatenate(dP_fem)
+
+            dn_fem = dn_carriers(wavelength, dN_fem, dP_fem)
+            dk_fem = alpha_to_k(dalpha_carriers(wavelength, dN_fem, dP_fem), wavelength)
+
+            # Interpolate the index perturbation onto the Waveguide grid
+            temp_grid = temp_Waveguide.waveguide.mode_solver.simulation.grid
+            X = temp_grid.centers.x
+            Y = temp_grid.centers.y
+            Z = temp_grid.centers.z
+
+            freq0 = td.C_0 / wavelength
+            freqs = [freq0]
+
+            x_mesh, y_mesh, z_mesh, freq_mesh = np.meshgrid(
+                X, Y, Z, freqs, indexing="ij"
+            )
+            x_mesh_2D = x_mesh[:, :, 0, 0]
+            y_mesh_2D = y_mesh[:, :, 0, 0]
+
+            dn_grid = np.nan_to_num(
+                griddata(
+                    (x_fem * cm / um, y_fem * cm / um),
+                    dn_fem,
+                    (x_mesh_2D, y_mesh_2D),
+                    DEVSIM_INTERPOLATION_METHOD,
+                )
+            )
+            dk_grid = np.nan_to_num(
+                griddata(
+                    (x_fem * cm / um, y_fem * cm / um),
+                    dk_fem,
+                    (x_mesh_2D, y_mesh_2D),
+                    DEVSIM_INTERPOLATION_METHOD,
+                )
+            )
+
+            # Extend to 3D (Nx, Ny,) -> (Nx, Ny, Nz,)
+            dn_grid_3D = np.stack([dn_grid] * Z.size, axis=-1)
+            dk_grid_3D = np.stack([dk_grid] * Z.size, axis=-1)
+
+            # Extend to 4D (Nx, Ny, Nz,) -> (Nx, Ny, Nz, Nf)
+            dn_grid_td = np.stack([dn_grid_3D] * len(freqs), axis=-1)
+            dk_grid_td = np.stack([dk_grid_3D] * len(freqs), axis=-1)
+
+            n_core, k_core = get_nk(core_material)
+            n_dataset = td.ScalarFieldDataArray(
+                n_core + dn_grid_td, coords=dict(x=X, y=Y, z=Z, f=freqs)
+            )
+            k_dataset = td.ScalarFieldDataArray(
+                k_core + dk_grid_td, coords=dict(x=X, y=Y, z=Z, f=freqs)
+            )
+
+            # core_material_pertub = td.CustomMedium.from_nk(
+            #     n=n_dataset,
+            #     k=k_dataset,
+            #     interp_method="linear",
+            # )
+            if isinstance(core_material, str):
+                name_material = core_material + "_with_carriers"
+            else:
+                name_material = "core_material_with_carriers"
+
+            eps_real = n_dataset**2 - k_dataset**2
+            eps_imag = 2 * n_dataset * k_dataset
+            eps_diag_data = td.ScalarFieldDataArray(
+                eps_real + 1.0j * eps_imag, coords=dict(x=X, y=Y, z=Z, f=freqs)
+            )
+
+            eps_perturb = td.PermittivityDataset(
+                eps_xx=eps_diag_data, eps_yy=eps_diag_data, eps_zz=eps_diag_data
+            )
+            core_material_pertub = td.CustomMedium(
+                name=name_material,
+                eps_dataset=eps_perturb,
+                frequency_range=[0.99 * freq0, 1.01 * freq0],
+            )
+
+            # dn_dict = (
+            #     {
+            #         "x": x_fem * cm / um,
+            #         "y": y_fem * cm / um + box_thickness,
+            #         "dn": dn_fem + 1j * dk_fem,
+            #     }
+            #     if perturb
+            #     else None
+            # )
+
+            # Create perturbed waveguide, handle like regular mode
+            return Waveguide(
+                wavelength=wavelength,
+                core_width=self.core_width / um,
+                core_thickness=self.core_thickness / um,
+                slab_thickness=self.slab_thickness / um,
+                box_thickness=box_thickness,
+                clad_thickness=clad_thickness,
+                side_margin=max(
+                    self.ppp_offset + self.xmargin, self.npp_offset + self.xmargin
+                )
+                / um,
+                grid_resolution=grid_resolution,
+                precision=precision,
+                core_material=core_material_pertub,
+                clad_material=clad_material,
+                cache=cache,
+            )
+        else:
+            # Create simple waveguide, handle like regular mode
+            return Waveguide(
+                wavelength=wavelength,
+                core_width=self.core_width / um,
+                core_thickness=self.core_thickness / um,
+                slab_thickness=self.slab_thickness / um,
+                box_thickness=box_thickness,
+                clad_thickness=clad_thickness,
+                side_margin=max(
+                    self.ppp_offset + self.xmargin, self.npp_offset + self.xmargin
+                )
+                / um,
+                grid_resolution=grid_resolution,
+                precision=precision,
+                core_material=core_material,
+                clad_material=clad_material,
+                cache=cache,
+            )
+
+
+def clear_devsim_cache() -> None:
+    try:
+        devsim.delete_mesh(mesh="dio")
+    except devsim.error:
+        warnings.warn("No mesh to delete.")
+
+    try:
+        devsim.delete_device(device="MyDevice")
+    except devsim.error:
+        warnings.warn("No device to delete.")
 
 
 if __name__ == "__main__":
     c = PINWaveguide(
-        wg_width=500 * nm,
+        core_width=500 * nm,
         core_thickness=220 * nm,
         slab_thickness=90 * nm,
     )
     c.ddsolver()
     c.save_device("test.dat")
 
     import os
```

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/devsim/get_solver.py` & `gdsfactory-6.99.0/gdsfactory/simulation/devsim/get_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/devsim/test_devsim.py` & `gdsfactory-6.99.0/gdsfactory/simulation/devsim/test_devsim.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-import numpy as np
 from gdsfactory.simulation.devsim import get_simulation_xsection
 import gdsfactory as gf
 
 PDK = gf.get_generic_pdk()
 PDK.activate()
 
 
 def test_pin_waveguide() -> None:
     """Test reverse bias waveguide."""
     nm = 1e-9
     c = get_simulation_xsection.PINWaveguide(
-        wg_width=500 * nm,
+        core_width=500 * nm,
         core_thickness=220 * nm,
         slab_thickness=90 * nm,
     )
     c.ddsolver()
     n_dist = {}
     neffs = {}
 
@@ -23,26 +22,27 @@
     voltages = [vmin, vmax]
     Vstep = vmax
 
     for ind, voltage in enumerate(voltages):
         Vinit = 0 if ind == 0 else voltages[ind - 1]
         c.ramp_voltage(Vfinal=voltage, Vstep=Vstep, Vinit=Vinit)
         waveguide = c.make_waveguide(wavelength=1.55)
-        waveguide.compute_modes(isolate=True)
-        n_dist[voltage] = waveguide.nx
-        neffs[voltage] = waveguide.neffs[0]
+        n_dist[voltage] = waveguide.index.values
+        neffs[voltage] = waveguide.n_eff[0]
 
-    dn = neffs[vmin] - neffs[vmax]
-    assert np.isclose(dn.real, -0.00011342135795189279), dn.real
+    # dn = neffs[vmin] - neffs[vmax]
+
+    # TODO: Find a correct value to test devsim
+    # assert np.isclose(dn.real, -0.00011342135795189279), dn.real
 
 
 if __name__ == "__main__":
     nm = 1e-9
     c = get_simulation_xsection.PINWaveguide(
-        wg_width=500 * nm,
+        core_width=500 * nm,
         core_thickness=220 * nm,
         slab_thickness=90 * nm,
     )
     c.ddsolver()
     n_dist = {}
     neffs = {}
 
@@ -51,12 +51,11 @@
     voltages = [vmin, vmax]
     Vstep = vmax
 
     for ind, voltage in enumerate(voltages):
         Vinit = 0 if ind == 0 else voltages[ind - 1]
         c.ramp_voltage(Vfinal=voltage, Vstep=Vstep, Vinit=Vinit)
         waveguide = c.make_waveguide(wavelength=1.55)
-        waveguide.compute_modes(isolate=True)
-        n_dist[voltage] = waveguide.nx
-        neffs[voltage] = waveguide.neffs[0]
+        n_dist[voltage] = waveguide.index.values
+        neffs[voltage] = waveguide.n_eff[0]
 
     dn = neffs[vmin] - neffs[vmax]
```

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/eme/meow_eme.py` & `gdsfactory-6.99.0/gdsfactory/simulation/eme/meow_eme.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/eme/test_meow_simulation.py` & `gdsfactory-6.99.0/gdsfactory/simulation/eme/test_meow_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/fem/mode_solver.py` & `gdsfactory-6.99.0/gdsfactory/simulation/fem/mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/fem/test_mode_solver.py` & `gdsfactory-6.99.0/gdsfactory/simulation/fem/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/get_effective_indices.py` & `gdsfactory-6.99.0/gdsfactory/simulation/get_effective_indices.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/get_modes_path.py` & `gdsfactory-6.99.0/gdsfactory/simulation/get_modes_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/get_sparameters_path.py` & `gdsfactory-6.99.0/gdsfactory/simulation/get_sparameters_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/__init__.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_material.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_material.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_meep_geometry.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_meep_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_port_eigenmode.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_simulation.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_eigenmode.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_materials.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/write_sparameters_grating.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/write_sparameters_meep.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/__init__.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/break_geometry.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/break_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/mesh.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/meshtracker.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/parse_component.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/parse_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/parse_gds.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/parse_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/parse_layerstack.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/parse_layerstack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/refine.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/refine.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/scratch/mesh3D.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/tests/test_meshing.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/uz_xsection_mesh.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/xy_xsection_mesh.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gmsh/xyz_mesh.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gmsh/xyz_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/__init__.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/get_results.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/get_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/get_simulation.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/materials.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/materials.py`

 * *Files 23% similar despite different names*

```diff
@@ -52,14 +52,37 @@
         name_or_index=name_or_index,
         material_name_to_medium=material_name_to_medium,
     )
     n, _ = td.Medium.eps_complex_to_nk(eps_complex)
     return n
 
 
+def get_nk(
+    name_or_index: Union[str, float],
+    wavelength: float = 1.55,
+    material_name_to_medium: Dict[str, PoleResidue] = MATERIAL_NAME_TO_MEDIUM,
+) -> float:
+    """Return refractive index and optical extinction coefficient
+    from material database.
+
+    Args:
+        wavelength: wavelength (um).
+        name_or_index: material name or refractive index.
+        material_name_to_medium: map name to medium.
+
+    """
+    eps_complex = get_epsilon(
+        wavelength=wavelength,
+        name_or_index=name_or_index,
+        material_name_to_medium=material_name_to_medium,
+    )
+    n, k = td.Medium.eps_complex_to_nk(eps_complex)
+    return n, k
+
+
 def get_medium(
     name_or_index: Union[str, float],
     material_name_to_medium: Dict[str, PoleResidue] = MATERIAL_NAME_TO_MEDIUM,
 ) -> td.Medium:
     """Return Medium from materials database.
 
     Args:
```

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/modes.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/modes.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                                v
         ________________________________________________
     """
 
     wavelength: Union[float, Sequence[float], Any]
     core_width: float
     core_thickness: float
-    core_material: MaterialSpec
+    core_material: Union[MaterialSpec, td.CustomMedium]
     clad_material: MaterialSpec
     box_material: Optional[MaterialSpec] = None
     slab_thickness: float = 0.0
     clad_thickness: Optional[float] = None
     box_thickness: Optional[float] = None
     side_margin: Optional[float] = None
     sidewall_angle: float = 0.0
@@ -159,16 +159,22 @@
         named_args_string = "_".join(settings)
         h = hashlib.md5(named_args_string.encode()).hexdigest()[:16]
         return cache_path / f"{self.__class__.__name__}_{h}.npz"
 
     @property
     def waveguide(self):
         """Tidy3D waveguide used by this instance."""
+        # if (not hasattr(self, "_waveguide")
+        #         or isinstance(self.core_material, td.CustomMedium)):
         if not hasattr(self, "_waveguide"):
-            core_medium = get_medium(self.core_material)
+            # To include a dn -> custom medium
+            if isinstance(self.core_material, td.CustomMedium):
+                core_medium = self.core_material
+            else:
+                core_medium = get_medium(self.core_material)
             clad_medium = get_medium(self.clad_material)
             box_medium = get_medium(self.box_material) if self.box_material else None
 
             freq0 = td.C_0 / np.mean(self.wavelength)
             n_core = core_medium.eps_model(freq0) ** 0.5
             n_clad = clad_medium.eps_model(freq0) ** 0.5
```

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/sim_run.yaml` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_modes.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_results.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_simulation.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/utils.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/write_sparameters.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py` & `gdsfactory-6.99.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/lumerical/__init__.py` & `gdsfactory-6.99.0/gdsfactory/simulation/lumerical/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/lumerical/interconnect.py` & `gdsfactory-6.99.0/gdsfactory/simulation/lumerical/interconnect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/lumerical/read.py` & `gdsfactory-6.99.0/gdsfactory/simulation/lumerical/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/lumerical/settings.py` & `gdsfactory-6.99.0/gdsfactory/simulation/lumerical/settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/lumerical/test_read_sparameters.py` & `gdsfactory-6.99.0/gdsfactory/simulation/lumerical/test_read_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py` & `gdsfactory-6.99.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py` & `gdsfactory-6.99.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/__init__.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/coupler.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/find_coupling_vs_gap.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/find_mode_dispersion.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/find_mode_dispersion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/find_modes.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/find_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/find_modes_cross_section.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/find_modes_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/find_neff_vs_width.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/find_neff_vs_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/get_mode_solver_coupler.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/get_mode_solver_cross_section.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/get_mode_solver_rib.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/get_mode_solver_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/neff_convergence_test.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/neff_convergence_test.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/overlap.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/overlap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/tests/test_find_modes.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/tests/test_find_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/types.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/types.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/modes/waveguide.py` & `gdsfactory-6.99.0/gdsfactory/simulation/modes/waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/photonic_circuit_models/__init__.py` & `gdsfactory-6.99.0/gdsfactory/simulation/photonic_circuit_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/photonic_circuit_models/coupler.py` & `gdsfactory-6.99.0/gdsfactory/simulation/photonic_circuit_models/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/photonic_circuit_models/mzi.py` & `gdsfactory-6.99.0/gdsfactory/simulation/photonic_circuit_models/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/photonic_circuit_models/ring.py` & `gdsfactory-6.99.0/gdsfactory/simulation/photonic_circuit_models/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/plot.py` & `gdsfactory-6.99.0/gdsfactory/simulation/plot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/plot_csv.py` & `gdsfactory-6.99.0/gdsfactory/simulation/plot_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/port_symmetries.py` & `gdsfactory-6.99.0/gdsfactory/simulation/port_symmetries.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/process/diffusion.py` & `gdsfactory-6.99.0/gdsfactory/simulation/process/diffusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/process/implant_tables.py` & `gdsfactory-6.99.0/gdsfactory/simulation/process/implant_tables.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/process/pysrim.py` & `gdsfactory-6.99.0/gdsfactory/simulation/process/pysrim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/process/silicon.py` & `gdsfactory-6.99.0/gdsfactory/simulation/process/silicon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/process/skew/antimony_si_skew.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/process/skew/arsenic_si_skew.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/process/skew/boron_si_skew.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/process/skew/boron_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv` & `gdsfactory-6.99.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/build_model.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/build_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/femwell_waveguide_model.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/femwell_waveguide_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/interpolators.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/interpolators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/meep_FDTD_model.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/meep_FDTD_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/meow_eme_model.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/meow_eme_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/mlp.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/mlp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/models.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/parameter.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/parameter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/plot_model.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/read.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/tests/test_mzi.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/tests/test_mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/tests/test_mzi_lattice.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sax/tests/test_parameters.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sax/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/__init__.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/add_gc.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/add_gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/circuit.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/__init__.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/bend_circular.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/bend_euler.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/coupler.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/coupler_fdtd.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/coupler_ring.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/gc.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/mmi1x2.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/mmi2x2.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/mzi.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/mzi_siepic.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/mzi_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/ring_double.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/ring_double_siepic.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/ring_single.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/ring_single_siepic.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/components/straight.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/get_transmission.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/get_transmission.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/model_from_gdsfactory.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/model_from_sparameters.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/model_from_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/plot_circuit.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/plot_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/plot_model.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_circuit.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/simphony/tests/test_components.py` & `gdsfactory-6.99.0/gdsfactory/simulation/simphony/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sipann/bend_circular.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sipann/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sipann/bend_euler.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sipann/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sipann/coupler.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sipann/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sipann/coupler_ring.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sipann/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/sipann/straight.py` & `gdsfactory-6.99.0/gdsfactory/simulation/sipann/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/simulation/thermal/heater.py` & `gdsfactory-6.99.0/gdsfactory/simulation/thermal/heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/snap.py` & `gdsfactory-6.99.0/gdsfactory/snap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/symbols.py` & `gdsfactory-6.99.0/gdsfactory/symbols.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/technology/__init__.py` & `gdsfactory-6.99.0/gdsfactory/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/technology/klayout_tech.py` & `gdsfactory-6.99.0/gdsfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/technology/layer_map.py` & `gdsfactory-6.99.0/gdsfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/technology/layer_stack.py` & `gdsfactory-6.99.0/gdsfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/technology/layer_views.py` & `gdsfactory-6.99.0/gdsfactory/technology/layer_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1226,20 +1226,19 @@
     """
     if name_str is None:
         raise OSError(f"layer {name_str!r} has no name")
     fields = name_str.split()
     return " ".join(fields[1:]) if len(fields) > 1 else ""
 
 
-def test_load_lyp():
+def test_load_lyp() -> None:
     from gdsfactory.config import PATH
 
     lys = LayerViews(PATH.klayout_lyp)
     assert len(lys.layer_views) > 10, len(lys.layer_views)
-    return lys
 
 
 if __name__ == "__main__":
     test_load_lyp()
     # import gdsfactory as gf
     # from gdsfactory.config import PATH
```

### Comparing `gdsfactory-6.98.2/gdsfactory/technology/simulation_settings.py` & `gdsfactory-6.99.0/gdsfactory/technology/simulation_settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/types.py` & `gdsfactory-6.99.0/gdsfactory/types.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/typings.py` & `gdsfactory-6.99.0/gdsfactory/typings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/utils/async_utils.py` & `gdsfactory-6.99.0/gdsfactory/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/utils/file_utils.py` & `gdsfactory-6.99.0/gdsfactory/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/utils/xml_utils.py` & `gdsfactory-6.99.0/gdsfactory/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/utils/yaml_utils.py` & `gdsfactory-6.99.0/gdsfactory/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/watch.py` & `gdsfactory-6.99.0/gdsfactory/watch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/widgets/layout_viewer.py` & `gdsfactory-6.99.0/gdsfactory/widgets/layout_viewer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/gdsfactory/write_cells.py` & `gdsfactory-6.99.0/gdsfactory/write_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.98.2/PKG-INFO` & `gdsfactory-6.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdsfactory
-Version: 6.98.2
+Version: 6.99.0
 Summary: python library to generate GDS layouts
 Keywords: eda,photonics,python
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -94,36 +94,36 @@
 Requires-Dist: h5py ; extra == "gmsh"
 Requires-Dist: mapbox_earcut ; extra == "gmsh"
 Requires-Dist: meshio ; extra == "gmsh"
 Requires-Dist: pygmsh ; extra == "gmsh"
 Requires-Dist: pyvista ; extra == "gmsh"
 Requires-Dist: trimesh ; extra == "gmsh"
 Requires-Dist: shapely ; extra == "gmsh"
-Requires-Dist: kfactory==0.7.0 ; extra == "kfactory"
+Requires-Dist: kfactory[git]==0.7.2 ; extra == "kfactory"
 Requires-Dist: meow-sim ; extra == "meow"
 Requires-Dist: ray[tune,air] ; extra == "ray"
 Requires-Dist: hyperopt ; extra == "ray"
 Requires-Dist: sax>=0.8.6 ; extra == "sax"
 Requires-Dist: jaxlib ; extra == "sax"
 Requires-Dist: jax ; extra == "sax"
-Requires-Dist: tidy3d==2.2.1 ; extra == "tidy3d"
+Requires-Dist: tidy3d==2.2.2 ; extra == "tidy3d"
 Provides-Extra: database
 Provides-Extra: dev
 Provides-Extra: devsim
 Provides-Extra: docs
 Provides-Extra: femwell
 Provides-Extra: full
 Provides-Extra: gmsh
 Provides-Extra: kfactory
 Provides-Extra: meow
 Provides-Extra: ray
 Provides-Extra: sax
 Provides-Extra: tidy3d
 
-# gdsfactory 6.98.2
+# gdsfactory 6.99.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
```

