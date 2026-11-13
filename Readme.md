# Cartesian Hand — STS3215 Redesign

A redesign of the [Cartesian Hand](https://github.com/generalroboticslab/Cartesian_Hand) (Duke University, General Robotics Lab) for **Feetech STS3215 servos**. The redesign keeps the original hand's function while substantially lowering assembly cost.

## What changed

The original Cartesian Hand is a 7-DoF, all-prismatic (linear-joint) end-effector that uses rack-and-pinion transmissions driven by Feetech-3915 servos. This version redesigns the hand around the much cheaper and widely available **STS3215** servo, reducing the cost of assembly while remaining equally functional.

## Cost comparison

| | Original (General Robotics Lab) | This redesign (STS3215) |
| --- | --- | --- |
| Servos | 7 × Feetech-3915 (≈ $57 each retail) | 7 × STS3215 (≈ $16 each) |
| Servo subtotal | ≈ $399 | ≈ $112 |
**Savings: roughly $278**

### How these numbers were obtained

- **Original, ≈ $500:** stated in the Cartesian Hand paper — structural parts about $30 in PLA, and the complete hand about $500 including seven servos, electronics, wiring and fasteners ([arXiv:2609.25696](https://arxiv.org/abs/2609.25696)).
- **Servo prices:** a retail listing for the Feetech HL-3915 shows about $65 each; the XLeRobot bill of materials lists the STS3215 at about $14 each (US). Prices vary by vendor, region, tariffs and quantity.
- **Redesign, ≈ $145:** estimated by taking the original's ≈ $500 total and swapping the servo cost (7 × $65 → 7 × $14). Everything else (printed parts, electronics, wiring, fasteners) is assumed to cost about the same. 

## Credit

Based on *The Cartesian Hand: In-Hand Manipulation with All-Linear Fingers* by Boxi Xia, Bokuan Li, Ryan Shin, Zijiang Yang, Jiaxun Liu and Boyuan Chen, Duke University General Robotics Lab. Original repository: <https://github.com/generalroboticslab/Cartesian_Hand> (Apache-2.0).

```
@misc{xia2026cartesianhandinhandmanipulation,
  title         = {The Cartesian Hand: In-Hand Manipulation with All-Linear Fingers},
  author        = {Boxi Xia and Bokuan Li and Ryan Shin and Zijiang Yang
                   and Jiaxun Liu and Boyuan Chen},
  year          = {2026},
  eprint        = {2609.25696},
  archivePrefix = {arXiv},
  primaryClass  = {cs.RO},
  url           = {https://arxiv.org/abs/2609.25696},
}
```

## License

Apache License 2.0, matching the original project.