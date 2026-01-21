# Awesome Rust Visualization

> Rust crates for data visualization and plotting.

The items on the list should be reusable crates (rather than one-off plot implementations that are coupled to particular datasets and are not designed to be reused).
I have initially populated this list with tools discovered via GitHub and crates.io (using both tags and keyword searches).

## Contents
- [Pure Rust](#pure-rust)
  - [wgpu-based tools](#wgpu-based)
  - [Coupled to GUI framework](#coupled-to-gui-framework)
  - [Terminal and ASCII outputs](#text-based-outputs)
- [Bindings to visualization rendering code in other languages](#bindings)
  - [Non-web-based](#non-web-based)
  - [Web-based](#web-based)


Please let me know (via issues or PRs) if I got any categorizations incorrect (I mostly did brief checks of the README or Cargo.toml for each crate).


## Pure Rust

By "Pure Rust", this means the __visualization logic__ is implemented in pure Rust. (Note that some of these are still "bindings" to lower-level graphics libraries like Cairo. Even WGPU could be considered a "binding" to the lower-level Metal/Vulkan/etc APIs.)


- https://github.com/plotters-rs/plotters
- https://github.com/SouthamptonRust/rustplot
- https://github.com/DougLau/splot
- https://github.com/coder543/dataplotlib
- https://github.com/limads/papyri
- https://github.com/ibrahimcesar/velociplot
- https://github.com/jonfres/fluent-plots
- https://github.com/BlondeBurrito/plotrs
- https://github.com/rtbo/plotive
- https://gitlab.com/Neek-sss/strafe/-/tree/master/strafe-plot

### WGPU-based

Crates that use [WGPU](https://github.com/gfx-rs/wgpu) for plotting.

- https://github.com/rerun-io/rerun
- https://github.com/jonmmease/avenger
- https://github.com/maplibre/maplibre-rs
- https://github.com/runmat-org/runmat/tree/main/crates/runmat-plot
- https://github.com/Ameyanagi/ruviz
- 
### Coupled to GUI framework

Crates in which the plot rendering is tightly coupled to a particular GUI framework. Some of these may also use WGPU for plotting, so this section may overlap somewhat with the "WGPU-based" section.

- https://github.com/Joylei/plotters-iced (iced)
- https://github.com/ulikoehler/liveplot-rs (egui)
- https://github.com/pierreaubert/gpui-toolkit/tree/main/gpui-px (gpui)
- https://github.com/bgkillas/kalc-plot (kalc, egui?)
- https://github.com/emilk/egui_plot (egui)
- https://github.com/donkeyteethUX/iced_plot (iced)
- https://github.com/JakkuSakura/gpui-plot (gpui)
- https://github.com/longbridge/gpui-component/tree/main/crates/ui/src/chart (gpui)
- https://github.com/eliotbo/bevy_plot (bevy)
- https://github.com/hacknus/bevy_voxel_plot (bevy)
- https://github.com/rtbo/plotive/tree/main/iced (iced)


### Text-based outputs

Crates focused on terminal and ASCII-based plotting.

- https://github.com/milliams/plot

## Bindings

This section includes bindings (to high-level visualization libraries implemented in other langauges).

### Non-web-based

These are bindings to plotting libraries implemented in other languages (e.g., Python), excluding web technologies (for these, see "Web-based" section below).

- https://github.com/cpmech/plotpy (matplotlib)
- https://github.com/SiegeLord/RustGnuplot (gnuplot)
- https://github.com/ploteria/ploteria (gnuplot)
- https://gitlab.com/ruivieira/matplotrust (matplotlib)
- https://github.com/sixalphaone/graphplot (typst)
- https://github.com/Latias94/dear-imgui-rs/tree/main/extensions/dear-implot (implot)
- https://github.com/DJDuque/pgfplots (latex)


### Web-based

- https://github.com/georgestagg/ggsql (vega-lite)
- https://github.com/procyon-rs/vega_lite_4.rs (vega-lite)
- https://github.com/wangjiawen2013/charton (vega-lite ?)
- https://github.com/cuprous-au/vega-view (vega-lite)
- https://github.com/alignoth/alignoth (vega-lite)
- https://github.com/plotly/plotly.rs (plotly)
- https://github.com/alceal/plotlars (plotly)
- https://github.com/yuankunzhang/charming (apache echarts)
- https://github.com/stevedonovan/flot-rs (flot)
- https://github.com/ondt/mapplot (google maps)
- https://github.com/micouy/plotka (multiple)


## Lower-level 2D and 3D rendering / general purpose graphics libraries

TODO: Does it make sense to include these in this list?

- https://github.com/gfx-rs/wgpu
- https://github.com/linebender/vello
- https://github.com/google/forma
- https://github.com/parasyte/pixels
- https://github.com/femtovg/femtovg
- https://github.com/dimforge/kiss3d
- https://github.com/MeadowlarkDAW/rootvg
- https://github.com/audulus/vger-rs
- https://github.com/UE2020/bufro
- https://github.com/schell/renderling
- https://github.com/BVE-Reborn/rend3
- https://github.com/DavidPeicho/albedo
- https://github.com/nannou-org/nannou
- https://github.com/AryanpurTech/BlueEngine
- https://github.com/ftilde/palace

## Related Lists

- [awesome-rust](https://github.com/rust-unofficial/awesome-rust)
- [awesome-webgpu](https://github.com/mikbry/awesome-webgpu)
- [awesome-biological-visualizations](https://github.com/keller-mark/awesome-biological-visualizations)
