# Research

> **Read this when** you need to explain what the Advanced Telerobotics Research Lab works on, which robots it uses or which projects are current and which are past.

The lab started with telepresence: robots that people operate from somewhere else and feel present in. It is now moving toward Physical AI: robots that sense, decide and act in the real world alongside people. This page covers that direction, the four message pillars with their proof points, current projects, platforms, past work with years and the programs that bring students in. Remember one rule: label past projects as past, with their years.

## Contents

- [From telepresence to Physical AI](#from-telepresence-to-physical-ai)
- [Four message pillars](#four-message-pillars)
- [Current projects](#current-projects)
- [Platforms](#platforms)
- [Past projects](#past-projects)
- [Programs](#programs)
- [Public code](#public-code)
- [Related](#related)

## From telepresence to Physical AI

**Where we come from.** The lab's name and first decade are about telepresence (driving a robot from somewhere else, seeing and hearing through it), tele-embodiment (feeling as if you are inside the robot's body while you control it) and immersive teleoperation (controlling a robot from a distance through virtual or augmented reality). The TeleBot line, the Telesuit control suit, the AARON augmented reality system for NASA SUITS and ImmersiFLY all come from this heritage.

**Where we are going.** New work leads with **Physical AI**: AI that senses and acts in the real world through a robot. A Physical AI agent is a robot that uses AI to perceive, decide and act, helping people with real tasks. The evidence is in the lab's recent choices:

- The 2026 summer programs are titled "Hands-on Physical AI & Robotics" for high school and for middle school students.
- New "Physical AI Agent" courses: undergraduate CS 4999X and graduate CS 5999Y, to be offered in 2027.
- A 2026 internship project area, "Physical AI Coworker": "Physical AI agents that assist humans in real-world tasks through perception, decision-making, and robotic interaction."
- The director's listed research interests: "Robotics, Telerobotics, Physical AI Agent, Human-Robot Interaction".
- Recent projects: VendoBot, Coffee Buddy, PepperKit and Expressive Motion (below).

**What connects the two.** People and robots sharing work, across a distance and side by side. In the lab's own words, the goal is "creating a cooperative world where robots help humans rather than replace them" (2021 news post).

> [!NOTE]
> Say "from telepresence to Physical AI" or "telepresence and Physical AI". Don't drop telepresence: it explains the lab's name. Don't claim leadership ("the leading Physical AI lab", "first", "only") without a source.

TeleBot itself began in 2012 at Florida International University under the director, before the lab existed. Attribute that early history to Jong-Hoon Kim, not to the lab.

## Four message pillars

Everything the lab publishes should serve one of these pillars. Proof points use the verified wording from [achievements.md](achievements.md).

| Pillar | What it means | Proof points |
|---|---|---|
| **1. Extending human presence** | Robots people operate and inhabit at a distance: telepresence, tele-embodiment, immersive VR and AR teleoperation | TeleBot-2 (World Robot Summit 2018); TeleBot-3R (the lab's World Robot Summit 2021 robot); TeleBot-4R and its Meta Quest XR interface (2023 to 2024); AARON, an AR system for NASA SUITS (selected as one of the top 10 teams for the onsite challenge in 2020; second generation built by the ATR_FLUX team in 2023); Telesuit (2019) |
| **2. Physical AI that works with people** | Robots that sense, decide and act in real settings alongside people: service robots, social robots, humanoids | VendoBot (HRI 2026 Companion, Edinburgh, March 2026); Coffee Buddy; PepperKit (Pepper with a realtime LLM voice agent); Expressive Motion on a Booster K1 (2026); Physical AI Agent courses; the "Physical AI Coworker" internship project |
| **3. Learning by building** | Students at every level do real research on real hardware and test it in competition | Undergraduate and graduate robotics courses; selected as one of 11 finalists in the World Robot Summit Plant Disaster Prevention Challenge (2021); selected as one of the top 10 teams for the onsite NASA SUITS challenge (2020); paper awards (IHCI 2020, IEMTRONICS 2020, IHCI 2023); hackathon results (2019); students from computer science to biomedical engineering and philosophy |
| **4. The next generation of innovators** | Hands-on robotics and Physical AI for middle and high school students and their teachers | 2025 and 2026 summer research internships; 2026 Summer Workshop; K-12 school workshops (2021, 2022); National Robotics Week open house (2019); partner lab in PRIDe, an NSF-funded K-12 computer science education project [confirm current role before use]; research on outreach (Cascade Mentoring, IHCI 2023) |

Plain terms used above: VR (virtual reality) is a fully digital view; AR (augmented reality) lays digital information over the real world; XR (extended reality) covers both. A humanoid is a robot shaped roughly like a person; a service robot does a job for people, such as delivering items.

## Current projects

### VendoBot

A projection-augmented delivery robot for improving intent transparency (showing people what the robot plans to do next) and motion legibility (moving in a way people can read and predict) in service robots. Published in the HRI 2026 Companion proceedings (Edinburgh, March 2026).

- Paper: [doi.org/10.1145/3776734.3794461](https://doi.org/10.1145/3776734.3794461) (full citation in [publications.md](publications.md#latest-verified-publication))
- Code: no public repository

### Coffee Buddy

An interactive service robot for coffee shop settings, with voice interaction, facial expressions and head tracking, built on ROS 2 (Robot Operating System, common open-source robot software).

- Code: [ATR-Lab/kami-head](https://github.com/ATR-Lab/kami-head) (the repository's README calls it the Coffee Buddy Robot)

### PepperKit

A SoftBank Pepper robot with a realtime LLM voice agent. An LLM (large language model) is an AI system trained on large amounts of text that generates written or spoken answers. Pepper streams what it hears to a backend service, which returns the answer Pepper speaks. Pepper's answers come from an AI language model and can be wrong.

- Code: [ATR-Lab/PepperKit](https://github.com/ATR-Lab/PepperKit) (a monorepo with the backend service, the Pepper Android client and a browser-based Android Studio environment)

### Expressive Motion

Expressive walking for a Booster K1 humanoid (2026). The pipeline turns a single video of a person walking into a reference motion that the K1 can be trained to imitate, aimed at robot fashion shows. Training uses simulation first (sim-to-real: train in simulation, then run on the real robot).

- Code, paper and poster: [ATR-Lab/expressive-motion](https://github.com/ATR-Lab/expressive-motion)

## Platforms

| Platform | What it is | Public code |
|---|---|---|
| SoftBank Pepper | A social robot (designed to talk and interact with people) | [ATR-Lab/PepperKit](https://github.com/ATR-Lab/PepperKit) |
| Unitree Go2 | A quadruped, or "robot dog" | [ATR-Lab/go2_ws](https://github.com/ATR-Lab/go2_ws): a ROS 2 workspace for controlling and interacting with Go2 robots |
| Booster K1 | A humanoid | [ATR-Lab/expressive-motion](https://github.com/ATR-Lab/expressive-motion) |
| Yahboom ROS 2 robot | The Yahboom R2L robot platform, running ROS 2 | [ATR-Lab/yahboom_r2l_ros2](https://github.com/ATR-Lab/yahboom_r2l_ros2): a ROS 2 port of the Yahboom R2L robot software |
| Robot mower | The lab's robot mower | [ATR-Lab/robo_mower_ws](https://github.com/ATR-Lab/robo_mower_ws): a ROS 2 workspace with camera, lidar, motor control and mapping |
| TeleBot-3R | The lab's World Robot Summit 2021 robot | No public repository |
| TeleBot-4R | A recent TeleBot generation (2023 to 2024), with an XR interface for Meta Quest headsets | [ATR-Lab/TeleBot-4R](https://github.com/ATR-Lab/TeleBot-4R) (ROS 2 code) and [ATR-Lab/TeleBot-4R-XR](https://github.com/ATR-Lab/TeleBot-4R-XR) (the XR interface) |

Where each robot is kept and how to book it is lab-internal information and is not published here. Lab members can start with the onboarding repo, [getting-started-atr-lab](https://github.com/ATR-Lab/getting-started-atr-lab).

## Past projects

These are finished. Describe them in the past tense, with their years.

| Project | Years | What it was |
|---|---|---|
| ImmersiFLY (Immersed Pilot Training Simulator) | 2017 to about 2019 | An immersive pilot training simulator |
| TeleBot-2 | 2018 | The TeleBot generation the lab demonstrated at the World Robot Summit in Tokyo (Plant Disaster Prevention Challenge) |
| Telesuit | 2019 | An immersive telepresence control suit, built with Kent State's Fashion School and its TechStyle Lab (2019 papers) |
| AARON for NASA SUITS | 2020, 2023 | An AR system for spacesuit operations. In 2020 a lab team was selected as one of the top 10 teams for the onsite NASA SUITS challenge; in 2023 the lab's ATR_FLUX team built the second generation |
| RoboCup 2023 teams | 2023 | The lab formed teams for RoboCup 2023 (RoboCup Rescue; RoboCup@Home Social Standard Platform League with Pepper) |
| Gesture-Enabled Telepresence Robot | [years] | [one-line description from the director] |
| MOVR | [years] | [one-line description from the director] |

> [!IMPORTANT]
> The lab website's "Current Project" block still shows ImmersiFLY. That block is stale: ImmersiFLY is a past project.

## Programs

| Program | Who it is for | What we can say |
|---|---|---|
| Courses | Undergraduate and graduate students | Undergraduate and graduate courses, including Human-Robot Interaction and Physical AI Agent (CS 4999X and CS 5999Y, to be offered in 2027); an undergraduate robotics course sequence (CS 23301 to CS 49995) |
| Summer research internship | High school students | Run in 2025 and 2026. A non-paid research experience in which students "learn how research ideas are developed, tested, and presented" (2026 internship page). Project areas include "Physical AI Coworker" |
| Summer workshop | Middle school students | 2026 Summer Workshop on Physical AI and Robotics. Details: [to be announced] |
| K-12 visits and workshops | Teachers and schools | The lab's offer: "We offer demos, learning sessions, and workshops." School workshops at Grand River Academy (2021) and Cleveland School of Science and Medicine (2022); a National Robotics Week open house (2019) |
| NSF PRIDe | K-12 computer science education | Partner lab in PRIDe, an NSF-funded K-12 computer science education project (2023 to 2027) [confirm current role before use] |

> [!WARNING]
> Programs for high school and middle school students involve minors. Never name a participant under 18, never pair a school name with a face and never post a photo without a signed parent or guardian release on file.

## Public code

The lab publishes code on GitHub as [ATR-Lab](https://github.com/ATR-Lab) (55 public repositories, counted Sept. 30, 2026). The repositories linked on this page were checked against their READMEs on that date. Many lab repositories are private; link only public ones.

## Related

- [Achievements](achievements.md): every result above, with the exact wording and its source
- [Publications](publications.md): VendoBot, the awarded papers and a selected list
- [Press kit](press-kit/README.md): boilerplates and a fact sheet built from the same facts
- [Members](members/README.md): who works on these projects
- [getting-started-atr-lab](https://github.com/ATR-Lab/getting-started-atr-lab): onboarding, lab rules and safety
- [all-things-ros2](https://github.com/ATR-Lab/all-things-ros2): ROS 2 guides for the lab's robots

<sub>Last reviewed: Sept. 30, 2026 · Sources checked on that date · [Suggest a change](https://github.com/ATR-Lab/about/edit/master/research.md)</sub>
