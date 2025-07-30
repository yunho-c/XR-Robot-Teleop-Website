---
title: 'XR-Robot-Teleop'
subtitle: 'a robot teleoperation client for VR/AR headsets'
# date: 2024-08-22
pinned: true
---

<script>
import Action from '$lib/Action.svelte'
import Button from '$lib/Button.svelte'
</script>

[`XR-Robot-Teleop`](https://github.com/yunho-c/XR-Robot-Teleop) is a **robot teleoperation client for VR/AR headsets** built in Unity. It uses [Meta Movement SDK](https://developers.meta.com/horizon/documentation/unity/move-body-tracking/) to obtain upper body poses (via [inside-out body tracking](https://developers.meta.com/horizon/blog/inside-out-body-tracking-and-generative-legs/)) and sends it to a user-specified IP address via WebRTC. 

[`XR-Teleop-Server`](https://github.com/yunho-c/XR-Teleop-Server) is a companion project written in Python that receives the body pose data. You can define custom callback functions (which are invoked every time the data is received) to visualize body poses or integrate into a robotic simulator. 

[TODO: demo selector & videos]

For more information, visit the [project page on GitHub](https://github.com/yunho-c/XR-Robot-Teleop).

<Action>
    <Button href="https://github.com/yunho-c/XR-Robot-Teleop">Download @ GitHub</Button>
    <!-- <Button href="https://TODO.com">Download @ Meta App Lab</Button> -->
</Action>
