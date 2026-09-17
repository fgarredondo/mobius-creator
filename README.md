# Mobius Creator

[Versión en español](README_ES.md)

**A repairable and modifiable delta 3D printer adapted to components available in Argentina.**

> **Current status:** active development and prototyping.
> No version has yet been released for fabrication.

![Mobius Creator main structure](https://github.com/user-attachments/assets/8bc3c71f-5907-4190-829e-2219b956a86d)

## Description

Mobius Creator is a large-format delta 3D printer project designed with an emphasis on repairability, spare-part availability, and user adaptability.

The goal is to develop a machine with considerable build volume and printing speed that can be built, maintained, modified, and repaired using standard components and alternatives available in the Argentine market whenever technically feasible.

The open release of the design files is planned once a sufficiently stable, documented, and validated configuration is available.

## Why did I choose a delta printer?

The choice of delta kinematics is mainly based on the ability to repeat the same mechanism across all three towers. By using three identical mechanical assemblies, the number of different parts that need to be designed, manufactured, tested, and maintained is reduced. An improvement made to the mechanism of one tower can be applied directly to the other two.

In the current configuration, each tower uses only three different models of 3D-printed parts. Their ends are integrated into the lower and upper structural bases.

As a result, the main structure, including the belt tensioners, can be built from four models of 3D-printed parts and four CNC-cut aluminum plates.

This low component diversity is intended to:

- Simplify manufacturing.
- Reduce the number of parts that need to be validated.
- Make spare parts easier to identify and store.
- Simplify assembly and maintenance.
- Allow improvements to be applied consistently across all three towers.

However, the choice was not purely technical. Ever since I first encountered delta printers, I have been fascinated by their fluid, hypnotic movements. That combination of mechanical repetition, speed, and motion eventually became a central part of Mobius Creator.
 
<img width="3300" height="2550" alt="Base assembly " src="https://github.com/user-attachments/assets/abb470a2-2a86-47c7-89b4-1313ba386a0f" />
<img width="2048" height="1536" alt="Belt tensioner " src="https://github.com/user-attachments/assets/59e2f0c5-1e4c-4e42-9827-b95167aa4b26" />
<img width="2048" height="1536" alt="Carriage" src="https://github.com/user-attachments/assets/3b429b73-4fd4-45d2-b7f4-8f37e9632786" />

## Project goals

The project prioritizes:

- Repairability and ease of maintenance.
- Local availability of spare parts.
- Use of standard components.
- Clear technical documentation.
- Publication of editable design files.
- Adaptability to different budgets and component availability.
- Validation through prototypes and documented testing.
- Identification of compatible alternatives for critical components.

## Preliminary specifications

The following characteristics represent the current state and goals of the development. They should not be considered final specifications.

- **Architecture:** Delta.
- **Target print diameter:** 350 mm.
- **Minimum target print height:** 350 mm.
- **Planned firmware:** Klipper.
- **Planned controller board for the first prototype:** BTT SKR Mini.
- **Planned control computer:** BTT Pi.
- **Planned extruder:** Sherpa Mini V3.
- **Planned ball joints:** IGUS KCLM-06-EK.
- **Planned arms:** 8 x 6 mm carbon-fiber tubes.
- **Planned endstops:** Optical.
- **Automatic bed leveling:** Using a removable nozzle-mounted accessory, similar to those used by BIQU or FLSUN.
- **Experimental hotend:** Creality K1 heatsink, titanium heat break, Volcano heater block, and CHT nozzle.
- **Experimental effector:** 3D-printed core reinforced with FR4 plates in a sandwich-type construction.

Speed, acceleration, flow rate, accuracy, and repeatability figures will be published once they can be verified through reproducible testing.

## Project status

Mobius Creator is currently in the development and prototyping phase. Files, dimensions, components, and mechanical solutions may change during this stage.

Versions prepared for fabrication will be explicitly identified and accompanied by the corresponding documentation.

### Current progress

- [x] Initial architecture defined.
- [x] Main structure and towers designed.
- [x] Belt tensioner designed and initially tested.
- [x] Preliminary carriage developed to validate motion and linear guides.
- [x] Preliminary electronics selected.
- [ ] First prototype structure fabricated (in progress).
- [ ] Effector designed and fabricated (in progress).
- [ ] Carriage design fully validated.
- [ ] Arms fabricated and measured.
- [ ] Electronics integrated.
- [ ] Initial Klipper configuration completed.
- [ ] Motion validated.
- [ ] Geometric calibration completed.
- [ ] First print completed.
- [ ] Repeatability and accuracy tests completed.
- [ ] First documented version prepared for external builders.

## Effector development

The effector is currently in the design stage. The preliminary configuration uses:

- IGUS KCLM-06-EK polymer ball joints.
- Sherpa Mini V3 extruder.
- Creality K1 heatsink.
- Titanium heat break.
- Volcano-style heater block.
- CHT nozzle.
- 3D-printed core reinforced with FR4 plates in a sandwich-type construction.

This combination is intended to keep the assembly compact and lightweight, simplify maintenance, and maintain an adequate material flow rate for large and fast prints.

The design will prioritize easy access to and replacement of its components. The configuration may change based on mechanical, thermal, and extrusion testing.

## Validation criteria

Before publishing the first reproducible version, the project is expected to evaluate at least:

- Positioning repeatability.
- Tower geometry and perpendicularity.
- Uniform carriage motion.
- Belt-system stability.
- Dimensional accuracy.
- Vibrations and resonances.
- Motor and electronics temperatures.
- Operation during extended prints.
- Ease of maintenance and component replacement.

Results will be identified as measured, estimated, or pending validation.

## Roadmap

### Stage 1: Mechanical prototype

- Complete the effector.
- Fabricate and measure the arms.
- Validate the carriages, guides, and tensioners.
- Verify the geometry of the structure.

### Stage 2: Integration

- Install the electronics.
- Prepare the wiring.
- Configure Klipper.
- Perform the first motion tests.

### Stage 3: Printing and testing

- Complete the first print.
- Fine-tune delta calibration.
- Measure repeatability and accuracy.
- Document failures and modifications.
- Perform extended printing tests.

### Stage 4: Reproducible release

- Freeze an experimental configuration.
- Publish the bill of materials.
- Publish versioned fabrication files.
- Prepare assembly instructions.
- Document known issues and warnings.
- Invite the first external builders.

## License

The project is currently in the development and prototyping phase. The licenses that will apply to the mechanical designs, electronics, software, and documentation have not yet been defined.

Unless expressly stated otherwise, publishing content in this repository does not grant permission to reproduce, modify, manufacture, distribute, or commercialize the published files or designs.

The final licenses will be announced before the first open and reproducible version of the project is released.

## Trademark

**Mobius Creator** is a registered trademark in Argentina.

The project name, logo, and other identifying elements will not automatically be included in any open licenses that may apply to the design files, software, or documentation.

Authorization to use the designs will not constitute authorization to market products under the Mobius Creator trademark.

## Warning

This project contains moving mechanical components, heated elements, electrical connections, and experimental systems that may present risks if manufactured, connected, or used incorrectly.

Experimental versions must not be considered finished designs or validated for production.

Before manufacturing or modifying any component:

1. Verify the file version.
2. Review the available documentation.
3. Check the known issues.
4. Verify dimensions, materials, and compatibility.
5. Do not leave the prototype operating unattended.

## Development images

### Upper tower support

![Upper tower support](https://github.com/user-attachments/assets/ba235d99-059a-4ee0-8339-9d9bb1cc3e29)

### Carriage detail

![Carriage detail](https://github.com/user-attachments/assets/0ae5da21-a42a-4deb-bd17-aea6d9d68dd7)

## Participation

The project is not yet at the public-build stage. However, feedback is welcome regarding:

- Component availability in Argentina.
- Experience with delta printers.
- Alternative components.
- Measurement and validation methods.
- Repairability.
- Technical documentation.
- Potential mechanical or maintenance issues.

Formal contribution guidelines will be published when the first reproducible experimental version is released.
