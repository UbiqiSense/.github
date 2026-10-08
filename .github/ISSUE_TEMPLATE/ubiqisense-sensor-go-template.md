---
name: Ubiqisense sensor-go template
about: Create a report to help us improve
title: 'sensor-go:'
labels: 'go'
assignees: ''
repository: 'sensor-go'
due date: ''
---

# 🐹 sensor-go Update / Issue Template

## 🧐 Why:
<!--
Describe the reason for this issue or change. What problem is it solving?
For a bug: what was observed, on which device (location / sensor id, platform) and when.
Paste the relevant log lines and the exact error message.
-->

## ✅ What:
<!--
Clearly outline what is being added, changed, or fixed.
Point to the code involved (internal/<package>/<file>.go:<line>) and include implementation details if relevant.
-->

## 🧭 Scope:
<!-- Tick everything that applies. -->
**Sensor mode:**
- [ ] OCCUPANCY
- [ ] FOOTFALL
- [ ] Both / mode-independent

**Platform:**
- [ ] RK3399 (arm64)
- [ ] Allwinner
- [ ] x86_64 / dev machine

**Area:** <!-- e.g. pipeline, video, ml, detection, footfall, calibration, cloud, shadow, buffer, config, snapshot, build/CI -->

## 🐍 Python Sensor parity:
<!--
Does the Python Sensor (UbiqiSense/Sensor) already do this, and must sensor-go behave the same?
Link the reference (e.g. Sensor/sensor_code/dnn_adapter.py:_generate_anchors) and state any intended difference.
For footfall counting, the reference is Footfall-Evaluation-Tool docs/COUNTING_SPEC.md and its golden cases.
-->

## ⚙️ Config & cloud contract:
<!--
Does this change configs/sensor.yaml keys, bootargs, the device shadow, IoT topics or payload fields?
Is it backward compatible with sensors and cloud consumers already deployed? Write "None" if not affected.
-->

## 📈 Device impact:
<!--
Expected effect on CPU, memory, disk, log volume or network on the device.
Include measurements (before / after) when performance is the point of the change.
-->

## 🔐 Security Considerations:
<!--
Are there any security implications?
New inputs, certificates or credentials, file permissions, privileges, network exposure?
-->

## 🧪 Testing:
<!--
How was this tested? Any edge cases?
- Unit tests: go test -race ./...
- Replay: cmd/replay on recorded data
- On device: which sensor(s), what was checked (logs, MQTT payloads, LED, snapshots)
-->

## 📎 Related:
<!--
Link related issues, PRs, docs (docs/migration.md section) and Python Sensor issues.
-->
