---
title: 'XR-Robot-Teleop-*'
subtitle: 'a robot teleoperation system for XR headsets'
# date: 2025-07-30
pinned: true
---

<script>
import Action from '$lib/Action.svelte'
import Button from '$lib/Button.svelte'
import GitHubLogo from "phosphor-svelte/lib/GithubLogo";
</script>


[`XR-Robot-Teleop-Client`](https://github.com/yunho-c/XR-Robot-Teleop-Client) is a **robot teleoperation client for VR/AR headsets** built in Unity. It uses [Meta Movement SDK](https://developers.meta.com/horizon/documentation/unity/move-body-tracking/) to obtain upper body poses (via [inside-out body tracking](https://developers.meta.com/horizon/blog/inside-out-body-tracking-and-generative-legs/)) and sends them to a user-specified IP address via WebRTC.

<!-- For more information, visit the [project page on GitHub](https://github.com/yunho-c/XR-Robot-Teleop-Client). -->

> ⚠️ Currently, `XR-Robot-Teleop-Client` only supports Meta Quest headsets.

<Action>
  <Button href="https://TODO.com">Download @ Meta App Lab</Button>
  <Button href="https://github.com/yunho-c/XR-Robot-Teleop-Client">
    <GitHubLogo size="24" color="#8B5CF6" weight="duotone" />
    GitHub
  </Button>
</Action>

[`XR-Robot-Teleop-Server`](https://github.com/yunho-c/XR-Robot-Teleop-Server) is a companion project written in Python that receives body pose data. You can define custom callback functions (which are invoked every time the data is received) to visualize or **integrate into a robotic simulator**. 

```bash
pip install xr-robot-teleop-server
```

<Action>
  <Button href="https://pypi.org/project/xr-robot-teleop-server">View @ PyPI</Button>
  <Button href="https://github.com/yunho-c/XR-Robot-Teleop-Server">
    <GitHubLogo size="24" color="#8B5CF6" weight="duotone" />
    GitHub
  </Button>
</Action>

### Demo

#### Teleop @ `MuJoCo`/`robosuite`

<br>

<iframe style="width: 100%; aspect-ratio: 16 / 9;" src="https://www.youtube.com/embed/R7ryrr48uPQ" title="SRL XR Dual Kinova Teleop Demo [7/28/2025]" frameborder="0" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

```
TODO: a Bibtex citation block (with click-to-copy for different citation formats) to Kong's paper
```

[Learn more](https://github.com/kczttm/robosuite) about the instantaneous pose calculation algorithm used here.

<br>

#### Viz w/ `rerun`

<br>

<iframe style="width: 100%; aspect-ratio: 16 / 9;" src="https://app.rerun.io/index.html?url=https://xr-robot-teleop-website.pages.dev/assets/body_pose_data_07282025_1126pm.rrd" title="XR-Robot-Teleop Rerun Visualization" ></iframe>

> `NOTE`: Set it to 1000 fps for real-time speed!

```
TODO: Fix the default FPS and get rid of log/warning sidebar
```

<br>
