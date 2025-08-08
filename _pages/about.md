---
permalink: /
title: "Portfolio"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---



Hi! I'm a robotics engineer with a deep curiosity for how machines perceive, learn, and act in the real world. My journey began with hands-on experimentation and quickly evolved into focused research during my thesis, where I collaborated with imec to explore practical applications of AI in robotics.

I thrive at the intersection of intelligent software and mechanical systems where algorithms leave the screen and meet reality. I’m especially drawn to challenges in computer vision, motion planning, and real-time decision-making for autonomous systems.

Beyond the technical side, I’m driven by the idea of building useful, meaningful systems tools that extend human capability, improve industry, or push what robots can do. I'm always learning, always building, and currently looking for opportunities to join teams that turn bold ideas into working machines.




Projects
======




Overview:

Developed a fully integrated, modular robotic framework enabling intelligent, adaptive grasping in complex, real-world environments with a focus on pharmaceutical production lines handling fragile and irregular items. The system introduces a new method in Physical AI, where the robot understands and leverages the physical properties of objects (e.g., mass, geometry, surface characteristics) to generalize the grasping task. This allows the robot to dynamically apply the necessary gripping force and strategy for each object, ensuring stability without causing damage. The framework combines Large Language Models (LLMs), vision-based pose estimation, force-based grasp control, and natural language interaction into a unified decision–perception–action loop. This framework was presented at the conference ITF World 2025 by imec, where it received strong feedback from robotics researchers and industry experts. The presentation is available on YouTube: [Watch my robotics demo on YouTube](https://www.youtube.com/watch?v=10evZqkg7gM) .

Key Features & Contributions:

1. Brain Module - LLM Decision Engine :

    - Integrated a custom prompting pipeline with ChatGPT to interpret human instructions, reason over perception data, and coordinate robot actions.

    - Enabled multi-turn dialogue for ambiguity resolution and intent clarification.

2. Perception Module - Object Detection & Pose Estimation :

    - Used FastSAM for segmentation and FoundationPose for precise pose estimation.

    - Fused RGB-D, spatial metadata, and LLM reasoning to robustly identify target objects even under occlusion or clutter.

3. Robot Module - Adaptive Motion Planning :

    - Implemented in C++ with ROS2 & MoveIt2, supporting multiple planners (RRT*, RRTConnect, CHOMP) for optimal, fast, or smooth motions.

    - Designed recovery strategies for failed plans, with predefined task-specific positions.

4. Voice Module - Speech Interaction :

    - Integrated ReSpeaker Mic 2.0 for real-time speech-to-text and ElevenLabs TTS for natural voice responses.

    - Enabled voice-controlled robot commands and verbal feedback to users.

5. Grasping Module - Force & Slip Adaptive Control :

    - Used new Melexis 3D force sensors for dynamic grip adjustment, slip detection, and object mass estimation.

    - Applied adaptive strategies to avoid damaging fragile pharmaceutical products.

Quantitative Achievements:

- ≥ 90% grasp success rate across diverse object sets.

- Pose estimation accuracy: ~2.5 cm position error, ≤ 8° orientation error.

- Speech recognition accuracy: 94% in quiet, 85% in noisy lab conditions.

- End-to-end task completion success: 85% for multi-step voice commands.

Impact:
This work demonstrates the feasibility of generalized, human-interactive robotic grasping using Physical AI, enabling robots to understand object properties and adapt grasping strategies accordingly. The framework is designed for safety-critical, high-precision environments, changing the way for intelligent automation in pharmaceuticals and other domains requiring careful object handling.


