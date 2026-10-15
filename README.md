# Swiss Post Voting System Tamarin Models

## Organization
### 1. **Models**
- `protocol1.spthy`: Tamarin model of the Swiss Post Voting System protocol (SPVS) without asymmetric encryption. Includes executability (*E*), Payload Accuracy (*A1-A14*), and assword Alteration (*P*) lemmas. All lemmas verify
- `protocol2.spthy`: Tamarin model of the Swiss Post Voting System protocol (SPVS) with asymmetric encryption. Includes executability (*E*), Payload Accuracy (*A1-A14*), and assword Alteration (*P*) lemmas. All lemmas verify
- `protocol1-i`: Folder containing variations of Protocol1 with 1 open channel with all lemmas - *E*, *A1-A14*, *P*:
    - `protocol1-i_Out_1.spthy` - Protocol1, open channel 1
    - `protocol1-i_Out_6.spthy` - Protocol1, open channel 6
    - `protocol1-i_Out_7.spthy` - Protocol1, open channel 7
    - `protocol1-i_Out_10.spthy` - Protocol1, open channel 10
    - `protocol1-i_Out_11a.spthy` - Protocol1, open channel 11a
    - `protocol1-i_Out_11b.spthy` - Protocol1, open channel 11b
    - `protocol1-i_Out_14.spthy` - Protocol1, open channel 14
    - `protocol1-i_Out_15.spthy` - Protocol1, open channel 15
    - `protocol1-i_Out_16.spthy` - Protocol1, open channel 16
    - `protocol1-i_Out_17.spthy` - Protocol1, open channel 17
    - `protocol1-i_Out_18_1.spthy` - Protocol1, open channel 18_1
    - `protocol1-i_Out_18_2.spthy` - Protocol1, open channel 18_2
    - `protocol1-i_Out_19.spthy` - Protocol1, open channel 19
- `protocol1-m / protocol1-i_Out_1_Out_11a_Out_11b_Out_7.spthy` - Protocol1 with multiple open channels - 1, 7, 11a, 11b with all lemmas - *E*, *A1-A14*, *P*
- `protocol2-i`: Folder containing variations of Protocol2 with 1 open channel with all lemmas - *E*, *A1-A14*, *P*:
    - `protocol2-i_Out_1.spthy` - Protocol2, open channel 1
    - `protocol2-i_Out_6.spthy` - Protocol2, open channel 6
    - `protocol2-i_Out_7.spthy` - Protocol2, open channel 7
    - `protocol2-i_Out_10.spthy` - Protocol2, open channel 10
    - `protocol2-i_Out_11a.spthy` - Protocol2, open channel 11a
    - `protocol2-i_Out_11b.spthy` - Protocol2, open channel 11b
    - `protocol2-i_Out_14.spthy` - Protocol2, open channel 14
    - `protocol2-i_Out_15.spthy` - Protocol2, open channel 15
    - `protocol2-i_Out_16.spthy` - Protocol2, open channel 16
    - `protocol2-i_Out_17.spthy` - Protocol2, open channel 17
    - `protocol2-i_Out_18_1.spthy` - Protocol2, open channel 18_1
    - `protocol2-i_Out_18_2.spthy` - Protocol2, open channel 18_2
    - `protocol2-i_Out_19.spthy` - Protocol2, open channel 19
- `protocol2-m / protocol2-i_Out_1_Out_11a_Out_11b_Out_7.spthy` - Protocol2 with multiple open channels - 1, 7, 11a, 11b with all lemmas - *E*, *A1-A14*, *P*
- `privacy` - Folder containing the models for VP1 and VP2 (table 2 for description of the honest/ malicious and present/ removed actors):
    - `protocol1_VP1.spthy` - Protocol1-VP1, proving lemmas *E, A1, A3, A5-6, A8, A10-12*
    - `protocol1-sVP1.spthy` - Protocol1-sVP1, proving lemmas *E, A1, A3, A5-6, A10-12*
    - `protocol1-sVP2.spthy` - Protocol1-sVP2, proving lemmas *E, P, A4, A6-A9*
    - `protocol1-VP2.spthy` - Protocol1-VP2, proving lemmas *E, P, A4, A6-A9*
    - `protocol2_VP1.spthy` - Protocol2-VP1, proving lemmas *E, A1, A3, A5-6, A8, A10-12*
    - `protocol2-sVP1.spthy` - Protocol2-sVP1, proving lemmas *E, A1, A3, A5-6, A10-12*
    - `protocol2-sVP2.spthy` - Protocol2-sVP2, proving lemmas *E, P, A4, A6-A9*
    - `protocol2-VP2.spthy` - Protocol2-VP2, proving lemmas *E, P, A4, A6-A9*
- `verifiability` - Folder containing the models for individual verifiability (IV) and universal verifiability (UV) (table 2 for description of the honest/ malicious and present/ removed actors)
    - `protocol1_IV.spthy` - Protocol1_IV, proving lemmas *E, A1, A3, A5-6, A8, A10-12*
    - `protocol1_UV.spthy` - Protocol1_UV, proving lemmas *E, P, A11-12*
    - `protocol1_xIV.spthy` - Protocol1_xIV, proving lemmas *E, A5-6, A10-12*
    - `protocol1-sIV.spthy` - Protocol1-sIV, proving lemmas *E, A1, A3, A5-6, A10-12*
    - `protocol1-sUV.spthy` - Protocol1-sUV, proving lemmas *E, A11-12*
    - `protocol2_IV.spthy` - Protocol2_IV, proving lemmas *E, A1, A3, A5-6, A8, A10-12*
    - `protocol2_UV.spthy` - Protocol2_UV, proving lemmas *E, P, A11-12*
    - `protocol2_xIV.spthy` - Protocol2_xIV, proving lemmas *E, A5-6, A10-12*
    - `protocol2-sIV.spthy` - Protocol2-sIV, proving lemmas *E, A1, A3, A5-6, A10-12*
    - `protocol2-sUV.spthy` - Protocol2-sUV, proving lemmas *E, A11-12*
2. **Oracles**
    - `protocol1.oracle`, `protocol1-i / protocol1.oracle`, and `protocol1-m / protocol1.oracle`: The oracles used to speed up the verification of *E, A1-A14, P* lemmas in Protocol1 and its variants with one and multiple open channels
    - `protocol2.oracle`, `protocol2-i / protocol2.oracle`, and `protocol2-m / protocol2.oracle`: The oracles used to speed up the verification of *E, A1-A14, P* lemmas in Protocol2 and its variants with one and multiple open channels
    - `privacy / protocol1_V.oracle` and `privacy / protocol1_V.oracle`: The oracles used to speed up the verification of *E, A1-A14, P* lemmas in the different privacy variants of Protocol1 and Protocol2
    - - `verifiability / protocol1_V.oracle` and `verifiability / protocol1_V.oracle`: The oracles used to speed up the verification of *E, A1-A14, P* lemmas in the different verifiability variants of Protocol1 and Protocol2

## Flags 
The flag `noHashCheck` allows the original Protocol1 and Protocol2 as well as their variants with one and multiple open channels to be run with the TCC (SCT) not performing an EB password check against the SCS hashes in the`SCT_verify_SCS_data` rule. To do that, the files can be run using `tamarin-prover interactive <protocolFileName> -DnoHashCheck --derivcheck-timeout=0` for the interactive version, or `tamarin-prover <protocolFileName> -DnoHashCheck --prove --derivcheck-timeout=0` for automatic verification.

We have also used the flag `complete` in the privacy and verifiability variants to easily exclude the parties we have marked as removed in table 2 of the paper.


## Reproducing The Results

The models have been tested with version 1.12.0 of the [tamarin-prover](https://github.com/tamarin-prover/tamarin-prover) (installation and usage guide available in chapter 2 of the [manual](https://tamarin-prover.com/manual/master/book/002_installation.html)).

To run the files, use the following commands:
- automatic: `tamarin-prover <protocolFileName> --prove --derivcheck-timeout=0`
    - e.g. to run it for protocol2.spthy: `tamarin-prover protocol2.spthy --prove --derivcheck-timeout=0`
- interactive: `tamarin-prover interactive <protocolFileName> --derivcheck-timeout=0`
    - e.g. to run it for protocol2.spthy: `tamarin-prover interactive protocol2.spthy --derivcheck-timeout=0` 
