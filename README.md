# Movement Lab

**Teaching humanoid robots to learn movement by watching humans.**

Movement Lab is a build-in-public project working toward a humanoid that can
observe human motion — dance, athletics, everyday dexterity — and learn to
reproduce it. The long-term north star is a robot that picks up movement the way
a person does: by watching, mimicking, and refining.

This repo is *stone one* of that vision — scoped small, built honestly, one
joint at a time.

## The North Star

A humanoid that learns physical skill from human demonstration: watch a salsa
lead, a jump, a gesture — retarget it onto the robot's body, refine it in
simulation, and eventually run it on real hardware. Ambitious on purpose. Built
incrementally on purpose.

## Where it is now

Early foundation, and growing in the open:
- Motion fundamentals in NumPy — poses, trajectories, velocity, acceleration
- First robot built, rendered, and animated in MuJoCo (a single-joint arm,
  swinging under generated motion)
- Next: multi-joint arms, then retargeting human motion onto a humanoid model

## The approach

The pipeline this is building toward, the same one behind modern humanoid skill
learning:

`human demonstration → retarget onto robot → refine in simulation → real hardware`

Core working principle: **generate → simulate → judge.** Code generates motion,
simulation surfaces problems cheaply before any hardware contact, and human
judgment decides whether the result is actually right.

## Built with

Python · NumPy · MuJoCo · Google Colab

## Why this project

Built by a professional humanoid-robot teleoperator — the demonstration data
this whole field learns from is what I work with daily. Movement Lab is where
that hands-on motion intuition meets the technical stack.
