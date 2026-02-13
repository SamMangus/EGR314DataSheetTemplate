---
title: Module's Selected Major Components
---

## Module's Selected Major Components

The following sections are the selected major components necessary for my subsystem that will be used to detect the temperature of water and then communicate that information to our control board.

### Power Management



### Sensor


### Component Selection

> Also acceptable, more markdown friendly

**Voltage Regulator**

1. MIC5501-3.0YM5-TR

    ![](VReg1.webp)

    * $0.12/each
    * [link to product](https://www.digikey.com/en/products/detail/microchip-technology/MIC5501-3-0YM5-TR/5277873)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Inexpensive                               | Requires external components and support circuitry for interface |
    | Compatible with PSoC                      | Needs special PCB layout.                                        |
    | Meets surface mount constraint of project |

2. MIC5504-3.3YM5-TR

    ![](VReg2.webp)

    * $0.16/each
    * [link to product](https://www.digikey.com/en/products/detail/microchip-technology/MIC5504-3-3YM5-TR/4864018)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Inexpensive                               | Requires external components and support circuitry for interface |
    | Compatible with PSoC                      | Needs special PCB layout.                                        |
    | Meets surface mount constraint of project |

3. AP2112K-3.3TRG1

    ![](VReg3.webp)

    * $0.22/each
    * [link to product](https://www.digikey.com/en/products/detail/diodes-incorporated/AP2112K-3-3TRG1/4470746)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Inexpensive                               | Requires external components and support circuitry for interface |
    | Compatible with PSoC                      | Needs special PCB layout.                                        |
    | Meets surface mount constraint of project |


**Rationale:** A clock oscillator is easier ...

**Temperature Sensor**

1. MIC5501-3.0YM5-TR

    ![](VReg1.webp)

    * $0.12/each
    * [link to product](https://www.digikey.com/en/products/detail/microchip-technology/MIC5501-3-0YM5-TR/5277873)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Inexpensive                               | Requires external components and support circuitry for interface |
    | 300 mA output                             | Outputs 3V possibly too low for my needs                         |
    | Meets surface mount constraint of project |

2. MIC5504-3.3YM5-TR

    ![](VReg2.webp)

    * $0.16/each
    * [link to product](https://www.digikey.com/en/products/detail/microchip-technology/MIC5504-3-3YM5-TR/4864018)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | 3.3V output                               | Supply voltage max of 6V                                         |
    | Small footprint                           | Needs special PCB layout.                                        |
    | Meets surface mount constraint of project |

3. AP2112K-3.3TRG1

    ![](VReg3.webp)

    * $0.22/each
    * [link to product](https://www.digikey.com/en/products/detail/diodes-incorporated/AP2112K-3-3TRG1/4470746)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Inexpensive                               | Requires external components and support circuitry for interface |
    | Compatible with PSoC                      | Needs special PCB layout.                                        |
    | Meets surface mount constraint of project |


**Rationale:** A clock oscillator is easier ...