---
title: 'XR-Robot-Teleop-Client'
subtitle: 'a robot teleoperation client for VR/AR headsets'
# date: 2024-08-22
pinned: true
---

<script>
import Action from '$lib/Action.svelte'
import Button from '$lib/Button.svelte'
</script>

<Action>
    <Button href="https://github.com/yunho-c/XR-Robot-Teleop-Client/releases">Download @ GitHub</Button>
    <Button href="https://TODO.com">Download @ Meta App Lab</Button>
</Action>

[`XR-Robot-Teleop-Client`](https://github.com/yunho-c/XR-Robot-Teleop-Client) is a **robot teleoperation client for VR/AR headsets** built in Unity. It uses [Meta Movement SDK](https://developers.meta.com/horizon/documentation/unity/move-body-tracking/) to obtain upper body poses (via [inside-out body tracking](https://developers.meta.com/horizon/blog/inside-out-body-tracking-and-generative-legs/)) and sends it to a user-specified IP address via WebRTC.

[`XR-Teleop-Server`](https://github.com/yunho-c/XR-Teleop-Server) is a companion project written in Python that receives the body pose data. You can define custom callback functions (which are invoked every time the data is received) to visualize body poses or integrate into a robotic simulator. 

For more information, visit the [project page on GitHub](https://github.com/yunho-c/XR-Robot-Teleop-Client).

> ⚠️ `XR-Robot-Teleop-Client` currently only supports Meta Quest headsets.


### Demo

#### Teleop @ `MuJoCo`/`robosuite`

<br>

<iframe style="width: 100%; aspect-ratio: 16 / 9;" src="https://www.youtube.com/embed/R7ryrr48uPQ" title="SRL XR Dual Kinova Teleop Demo [7/28/2025]" frameborder="0" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

TODO: a Bibtex citation block (with click-to-copy for different citation formats) to Kong's paper

Learn more about this project [here](https://github.com/kczttm/robosuite).

<br>

#### Viz w/ `rerun`

<br>

<iframe style="width: 100%; aspect-ratio: 16 / 9;" src="https://app.rerun.io/index.html?url=https://xr-robot-teleop-website.pages.dev/assets/body_pose_data_07282025_1126pm.rrd" title="XR-Robot-Teleop Rerun Visualization" ></iframe>

(NOTE: Set it to 1000 fps!)
(TODO: Fix the default FPS and get rid of log/warning sidebar)

<br>
