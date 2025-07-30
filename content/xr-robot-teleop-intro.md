---
title: 'XR-Robot-Teleop'
subtitle: 'a robot teleoperation client for VR/AR headsets'
# date: 2024-08-22
pinned: true
---

<script>
import Action from '$lib/Action.svelte'
import Button from '$lib/Button.svelte'
import Tabs from '$lib/Tabs.svelte';

	let tabs = {
		'Live Demo': live_demo,
		'Pre-recorded': pre_recorded
	};
</script>

[`XR-Robot-Teleop`](https://github.com/yunho-c/XR-Robot-Teleop) is a **robot teleoperation client for VR/AR headsets** built in Unity. It uses [Meta Movement SDK](https://developers.meta.com/horizon/documentation/unity/move-body-tracking/) to obtain upper body poses (via [inside-out body tracking](https://developers.meta.com/horizon/blog/inside-out-body-tracking-and-generative-legs/)) and sends it to a user-specified IP address via WebRTC.

[`XR-Teleop-Server`](https/github.com/yunho-c/XR-Teleop-Server) is a companion project written in Python that receives the body pose data. You can define custom callback functions (which are invoked every time the data is received) to visualize body poses or integrate into a robotic simulator.

{#snippet live_demo()}
	<!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->
    <p>a</p>
{/snippet}

{#snippet pre_recorded()}
	<!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/o-YBDTqX_ZU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->
    <p>b</p>
{/snippet}

<Tabs {tabs} />

For more information, visit the [project page on GitHub](https://github.com/yunho-c/XR-Robot-Teleop).

<Action>
    <Button href="https://github.com/yunho-c/XR-Robot-Teleop/releases">Download @ GitHub</Button>
    <!-- <Button href="https://TODO.com">Download @ Meta App Lab</Button> -->
</Action>
