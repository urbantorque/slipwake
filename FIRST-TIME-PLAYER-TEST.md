# Fairwater: player and device checks

Run five to eight fresh-player sessions. Observe the first ten minutes and any voluntary continuation. Use a fresh browser profile, because starting local notes preserves game progress. Settings > Playtest notes starts an opt-in, memory-only recording. Record the physical device, input, racing experience and any help in the notes. A browser reload discards the recording unless it has been exported.

Say: “Play for as long as you want. Tell me what you are trying to do.” Let the player choose their route through the game. Record time to the first driving control, first drift release, Wake capture, full charge, actual Wake burst and completed pass. After play, ask what caused the burst, whether it was intentional and whether they deliberately repeated the sequence. Enter their exact explanation and both intent answers separately. Two recorded passes are an observation, not proof of mastery.

The first 64 and latest 176 observations are retained. Counters and first-event timings cover the whole recording, including events omitted from the bounded list. `firstAt.second-pass` is the time of a second actual pass across the recording, without a claim about intent. `boost:draft` counts real Wake launches, including bursts that did not become a completed pass. Note pauses, coaching and help when interpreting wall-clock timings.

After the unprompted portion, offer one directed licence attempt. Ask the player to state its goal. Observe a near miss or recovery/contact-limit failure, the primary retry action, the next destination after success, and a completed three-destination paint reward. A livery preview is temporary; the fit-and-race action saves the paint. Confirm that the fitted equipment and unfinished Cup are preserved. Directed tasks are separate from voluntary replay evidence.

Watch Lantern shoulder exchanges and counterattacks. Ask which rival they remember, whether a hit felt avoidable, and which visual or sound warned them. Check cannon warning direction on keyboard speakers, headphones and a physical controller. Record discomfort, confusion and stopping reasons in the player's words. Automatic event counts cannot establish fairness or enjoyment.

## Physical-device performance

Agree a named recommended laptop/phone and a named minimum laptop/phone before setting a release gate. Proposed targets are 60 fps on the recommended set and stable 30 fps on the minimum set. Record device model, OS/browser, input, quality, viewport/DPR, power mode and whether the device is warm. These hardware sessions remain pending until someone actually performs them.

1. Play a complete Cup on the actual device, including a crowded start, nearby items and Lantern bends. From pause > Settings > Playtest notes, save the live-race performance snapshot. It includes CPU phases and recent presentation intervals. These samples may include adaptive-scale changes; retain the reported buffer size and scale.
2. In the same panel, enter a device/input label and choose the render target. Run **Measure fixed scene**. It uses a separate stock six-boat view at seed 13721 and course fraction 0.17. The race stays paused. Two seconds settle the camera/shaders; eight seconds measure full-rate rendering at held resolution. Save the scene measurement. Repeat three times with the same course, quality, viewport and scale, alternating build order for comparisons. A viewport/visibility change cancels the run.
3. The fixed scene isolates rendering and excludes simulation, music and input latency. Its selected-budget result applies only to this render scene. Use the live-race trace and sustained play to judge the complete game.
4. Check touch steering/Slow/Drift with actual fingers. Record missed inputs, hand obstruction and perceived delay. For a measured input-to-visible-response delay, film the physical input and display together at high frame rate and count frames; report the capture rate and uncertainty. CPU render submission timing is not GPU duration or end-to-end input latency.

CPU slowdown, phone viewports and virtual controllers are engineering probes. Report them separately from physical hardware and fresh-player sessions. Keep failed and slower samples. Rank the three largest observed replay blockers before commissioning another feature pass.
