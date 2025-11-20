# QXDM_0xB821_0xB950_to_OAI_conf

online calculator: https://dustinchen26.github.io/QXDM_0xB821_0xB950_to_OAI_conf

## How to use
```
把QXDM[0xB821][0xB950]複製貼到輸入框，即可解析出OAI conf，記得QXDM Options->Export Parsed Text
```
## Example Input
```
06:38:45.373934          OTA LOG                  [0xB821]                 BCCH_DL_SCH / SystemInformationBlockType1                   BCCH_DL_SCH / SystemInformationBlockType1
06:38:45.373934
06:38:45.373934	[0xB821]	BCCH_DL_SCH / SystemInformationBlockType1
Pkt Version = 23
RRC Release Number.Major.minor = 17.4.0
Radio Bearer ID = 0, Physical Cell ID = 186
NR Cell Global ID = 0
Freq = 720288
Sfn = 992, SubFrameNum = 0
slot = 1
PDU Number = BCCH_DL_SCH Message,    Msg Length = 111
SIB Mask in SI =  0x02
ChoId = N/A
Segmented PDU = false
Last Segment = NA
Segment Index = NA
Interpreted PDU:

value BCCH-DL-SCH-Message ::= 
{
  message c1 : systemInformationBlockType1 : 
      {
        cellSelectionInfo 
        {
          q-RxLevMin -70,
          q-QualMin -25
        },
        cellAccessRelatedInfo 
        {
          plmn-IdentityInfoList 
          {
            {
              plmn-IdentityList 
              {
                {
                  mcc 
                  {
                    0,
                    0,
                    1
                  },
                  mnc 
                  {
                    0,
                    1
                  }
                }
              },
              trackingAreaCode '00000000 00000000 00000001'B,
              cellIdentity '00000000 00000000 10011110 00000000 0001'B,
              cellReservedForOperatorUse notReserved
            }
          }
        },
        si-SchedulingInfo 
        {
          schedulingInfoList 
          {
            {
              si-BroadcastStatus broadcasting,
              si-Periodicity rf32,
              sib-MappingInfo 
              {
                {
                  type sibType2,
                  valueTag 0
                },
                {
                  type sibType4,
                  valueTag 0
                },
                {
                  type sibType5,
                  valueTag 0
                }
              }
            }
          },
          si-WindowLength s5
        },
        servingCellConfigCommon 
        {
          downlinkConfigCommon 
          {
            frequencyInfoDL 
            {
              frequencyBandList 
              {
                {
                  freqBandIndicatorNR 79
                }
              },
              offsetToPointA 0,
              scs-SpecificCarrierList 
              {
                {
                  offsetToCarrier 0,
                  subcarrierSpacing kHz30,
                  carrierBandwidth 273
                }
              }
            },
            initialDownlinkBWP 
            {
              genericParameters 
              {
                locationAndBandwidth 1099,
                subcarrierSpacing kHz30
              },
              pdcch-ConfigCommon setup : 
                {
                  controlResourceSetZero 0,
                  searchSpaceZero 0,
                  commonSearchSpaceList 
                  {
                    {
                      searchSpaceId 1,
                      controlResourceSetId 0,
                      monitoringSlotPeriodicityAndOffset sl1 : NULL,
                      monitoringSymbolsWithinSlot '10000000 000000'B,
                      nrofCandidates 
                      {
                        aggregationLevel1 n0,
                        aggregationLevel2 n0,
                        aggregationLevel4 n4,
                        aggregationLevel8 n2,
                        aggregationLevel16 n1
                      },
                      searchSpaceType common : 
                        {
                          dci-Format0-0-AndFormat1-0 
                          {
                          }
                        }
                    }
                  },
                  searchSpaceSIB1 0,
                  searchSpaceOtherSystemInformation 1,
                  pagingSearchSpace 1,
                  ra-SearchSpace 1
                },
              pdsch-ConfigCommon setup : 
                {
                  pdsch-TimeDomainAllocationList 
                  {
                    {
                      mappingType typeA,
                      startSymbolAndLength 53
                    },
                    {
                      mappingType typeA,
                      startSymbolAndLength 44
                    },
                    {
                      mappingType typeA,
                      startSymbolAndLength 81
                    }
                  }
                }
            },
            bcch-Config 
            {
              modificationPeriodCoeff n2
            },
            pcch-Config 
            {
              defaultPagingCycle rf32,
              nAndPagingFrameOffset oneSixteenthT : 3,
              ns one,
              firstPDCCH-MonitoringOccasionOfPO sCS480KHZoneT-SCS120KHZquarterT-SCS60KHZoneEighthT-SCS30KHZoneSixteenthT : 
                {
                  2
                }
            }
          },
          uplinkConfigCommon 
          {
            frequencyInfoUL 
            {
              scs-SpecificCarrierList 
              {
                {
                  offsetToCarrier 0,
                  subcarrierSpacing kHz30,
                  carrierBandwidth 273
                }
              },
              p-Max 23
            },
            initialUplinkBWP 
            {
              genericParameters 
              {
                locationAndBandwidth 1099,
                subcarrierSpacing kHz30
              },
              rach-ConfigCommon setup : 
                {
                  rach-ConfigGeneric 
                  {
                    prach-ConfigurationIndex 198,
                    msg1-FDM one,
                    msg1-FrequencyStart 2,
                    zeroCorrelationZoneConfig 10,
                    preambleReceivedTargetPower -90,
                    preambleTransMax n20,
                    powerRampingStep dB4,
                    ra-ResponseWindow sl20
                  },
                  ssb-perRACH-OccasionAndCB-PreamblesPerSSB one : n32,
                  groupBconfigured 
                  {
                    ra-Msg3SizeGroupA b144,
                    messagePowerOffsetGroupB dB0,
                    numberOfRA-PreamblesGroupA 4
                  },
                  ra-ContentionResolutionTimer sf64,
                  rsrp-ThresholdSSB 0,
                  prach-RootSequenceIndex l139 : 4,
                  msg1-SubcarrierSpacing kHz30,
                  restrictedSetConfig unrestrictedSet
                },
              pusch-ConfigCommon setup : 
                {
                  pusch-TimeDomainAllocationList 
                  {
                    {
                      k2 1,
                      mappingType typeA,
                      startSymbolAndLength 27
                    },
                    {
                      k2 2,
                      mappingType typeA,
                      startSymbolAndLength 27
                    },
                    {
                      k2 3,
                      mappingType typeA,
                      startSymbolAndLength 27
                    },
                    {
                      k2 4,
                      mappingType typeA,
                      startSymbolAndLength 27
                    },
                    {
                      k2 5,
                      mappingType typeA,
                      startSymbolAndLength 27
                    }
                  },
                  msg3-DeltaPreamble 0,
                  p0-NominalWithGrant -78
                },
              pucch-ConfigCommon setup : 
                {
                  pucch-ResourceCommon 12,
                  pucch-GroupHopping neither,
                  p0-nominal -96
                }
            },
            timeAlignmentTimerCommon infinity
          },
          ssb-PositionsInBurst 
          {
            inOneGroup '10000000'B
          },
          ssb-PeriodicityServingCell ms20,
          tdd-UL-DL-ConfigurationCommon 
          {
            referenceSubcarrierSpacing kHz30,
            pattern1 
            {
              dl-UL-TransmissionPeriodicity ms2p5,
              nrofDownlinkSlots 3,
              nrofDownlinkSymbols 6,
              nrofUplinkSlots 2,
              nrofUplinkSymbols 4,
              dl-UL-TransmissionPeriodicity-v1530 ms3
            },
            pattern2 
            {
              dl-UL-TransmissionPeriodicity ms2,
              nrofDownlinkSlots 4,
              nrofDownlinkSymbols 0,
              nrofUplinkSlots 0,
              nrofUplinkSymbols 0
            }
          },
          ss-PBCH-BlockPower -11
        },
        ims-EmergencySupport true,
        ue-TimersAndConstants 
        {
          t300 ms1000,
          t301 ms200,
          t310 ms1000,
          n310 n10,
          t311 ms10000,
          n311 n1,
          t319 ms1000
        }
      }
}
06:38:45.381304          LOG                      [0xB950]                 NR5G ML1 DL Common Config                                   Length:   56
06:38:45.381304
06:38:45.381304	[0xB950]	NR5G ML1 DL Common Config
Major.Minor Version = 3. 2
Version 0x30002
   Current SFN time
      Slot = 1
      Sub FN = 8
      Sys FN = 992
      SCS = 30KHZ
   OTA Cfg Param
      Logging time Sub FN = 8
      Logging time Sys FN = 992
      Num cg add mod = 1
      CG Add Mod
         Log mask = 0
         Common Cg Config[0]
            Cell group Id = 0
            Target Dl Cell Frequency = 720288
            Target Phy Cell Id = 186
            CFG Mask = MAIN
            CC Id Del Bmask = 0
            CC Id addmod bmask = 1
            RLM in sync out of sync threshold = 0
            Mac main CFG[0] {
               Is Cdrx Config Present = 0
            }
06:38:45.381338          LOG                      [0xB950]                 NR5G ML1 DL Common Config                                   Length:  712
06:38:45.381338
06:38:45.381338	[0xB950]	NR5G ML1 DL Common Config
Major.Minor Version = 3. 2
Version 0x30002
   Current SFN time
      Slot = 1
      Sub FN = 8
      Sys FN = 992
      SCS = 30KHZ
   OTA Cfg Param
      Logging time Sub FN = 8
      Logging time Sys FN = 992
      Num cg add mod = 1
      CG Add Mod
         Log mask = 1
         Per CC Config[0]
            Cell Info
               Band = BAND79
               Phy Cell Id = 186
               SSB Sub Carrier Spacing = 30KHZ
               DL Cell frequency = 720288
            Duplex Mode = TDD
            SCC Id = 0
            serv_cell_idx = 0
            num_coreset_add_mod = 2
            num_search_space_add_mod = 2
            num_dl_bwp_id_addmod = 1
            num_ul_bwp_id_addmod = 1
            dl_bwp_id_rel_bmask = 0
            dl_bwp_id_addmod_bmask = 1
            ul_bwp_id_rel_bmask = 0
            ul_bwp_id_addmod_bmask = 1
            cfg_mask = COMMON | DEDICATED | DL FREQUENCY INFO | UL FREQUENCY INFO
            CC Common CFG[0]
               dmrs_type_a_pos = NR5G_DL_DMRS_ADD_POS_2
               SS PBCH BLK PWR = -11
               SSB Period = MS20
               Rate Match Pattern Id Rel Bmask = 0
               Rate Match Pattern Add Mod Mask = 0
               CFG Mask = SSB_POS_BURST | SUB_CAR_SPACING | TDD_UL_DL | 0x10
               Sub Carr Spacing = 30KHZ
               SSB POS In Burst Bmask = 8000000000000000
               TDD UL DL CFG[0]
                  Enable = 1
                  Ref Scs = 1
                  Pattern2 Enable = 1
                  Pattern 1
                     DL Ul trans Period = MS5
                     Num DL Sym = 6
                     Num Ul Sym = 4
                     Num DL Slots = 3
                     Num Ul Slots = 2
                  Pattern 2
                     DL Ul trans Period = MS2
                     Num DL Sym = 0
                     Num Ul Sym = 0
                     Num DL Slots = 4
                     Num Ul Slots = 0
            CC Dedicated CFG[0]
               Tag Id = 0
               BWP Inact Timer = MS0,
               First Active DL bwp Id = 0
               Default Dl Bwp Id = 0
               First Active Ul Bwp = 0
               UE Beam lock Fn = 0
               Serving Cell mo id = 0
               CFG Mask = 0
               Path loss Reference linking = PCELL
               Antenna Info DL
                  Max Mimo Lyr Cfged = 1
                  Max Num Mimo Lyr = LYR_FOUR
                  Max Num rx = FOUR
            DL Frequency Info[0]
               Abs Freq SSB = 720288
               Abs Freq Point A = 720048
               Num Scs Carriers = 1
               Multi frequency Band List
                  Num Bands = 1
                  Frequency Band Indicator = { 79, 0, 0, 0, 0, 0, 0, 0 }
               Scs Spec Carrier List
                  -------------------------------------------------
                  |   |Offset To |Carrier BW|          |          |
                  |#  |Carrier   |Prb       |SCS       |Carrier BW|
                  -------------------------------------------------
                  |  0|         0|       273|     30KHZ|    100MHZ|
                  |  1|         0|         0|     15KHZ|      5MHZ|
                  |  2|         0|         0|     15KHZ|      5MHZ|
                  |  3|         0|         0|     15KHZ|      5MHZ|
                  |  4|         0|         0|     15KHZ|      5MHZ|

            UL Frequency Info[0]
               Abs Freq Point A = 720048
               P Max = 230
               Add Spectrum emission Present = 0
               Add Spectrum Emission = 0
               Freq Shift 7p5_khz = 0
               Num SCS Carriers = 1
               Multi Frequency band List
                  Num Bands = 1
                  Frequency Band Indicator = { 79, 0, 0, 0, 0, 0, 0, 0 }
               Scs Spec Carrier List
                  -------------------------------------------------
                  |   |Offset To |Carrier BW|          |          |
                  |#  |Carrier   |Prb       |SCS       |Carrier BW|
                  -------------------------------------------------
                  |  0|         0|       273|     30KHZ|    100MHZ|
                  |  1|         0|         0|     15KHZ|      5MHZ|
                  |  2|         0|         0|     15KHZ|      5MHZ|
                  |  3|         0|         0|     15KHZ|      5MHZ|
                  |  4|         0|         0|     15KHZ|      5MHZ|

            DL BWP Params[0] {
               BWP Generic Params
                  BWP Id =          0
                  Loc And BW =       1099
                  Sub Carrier Spacing =      30KHZ
                  Cyclic Prefix =     NORMAL
               CFG mask = COMMON | DEDICATED
               DL BWP Common[0]
                  CFG Mask = MASK PDCCH | MASK PDSCH
                  Pdcch Common[0]
                     Enable = 1
                     Coreset Zero Id = 0
                     Search Space Zero Id = 0
                     Coreset Active bmask = 1
                     Coreset Release Bmask = 0
                     Search Space Active Bmask = 0000000000000003
                     Search Space Rel Bmask = 0000000000000000
                     Search Space Id RMSI = 0
                     Search Space ID OSI = 1
                     Search Space ID Paging = 1
                     Search Space ID RA = 1
                  Pdsch Common[0]
                     Enable = 1
                     Num Pdsch Alloc List = 3
                     Pdsch Time Dom Alloc List
                        -------------------------------------------------
                        |   |          |Mapping   |          |Start Sum |
                        |#  |K Present |type      |K         |and length|
                        -------------------------------------------------
                        |  0|         0|    TYPE A|         0|        53|
                        |  1|         0|    TYPE A|         0|        44|
                        |  2|         0|    TYPE A|         0|        81|
                        |  3|         0|    TYPE A|         0|         0|
                        |  4|         0|    TYPE A|         0|         0|
                        |  5|         0|    TYPE A|         0|         0|
                        |  6|         0|    TYPE A|         0|         0|
                        |  7|         0|    TYPE A|         0|         0|
                        |  8|         0|    TYPE A|         0|         0|
                        |  9|         0|    TYPE A|         0|         0|
                        | 10|         0|    TYPE A|         0|         0|
                        | 11|         0|    TYPE A|         0|         0|
                        | 12|         0|    TYPE A|         0|         0|
                        | 13|         0|    TYPE A|         0|         0|
                        | 14|         0|    TYPE A|         0|         0|
                        | 15|         0|    TYPE A|         0|         0|

               DL BWP Dedicated[0]
                  CFG Mask = PDSCH
                  Pdsch CFG DED[0]
                     Enable = 1
                     Mcs Table = 64QAM
                     Rbg Size = 1
                     CFG Mask = DATA SCR ID | DMRS DL TYPEA
                     Pdsch Rsc Alloc = RATP1
                     Max Code words Scheduled by DCI = N1
                     Vrb to Prb InterLeaver = NONE
                     Data Scr Id = 65535
                     Rate Match Pattern1 Cell Level Id bmask = 0
                     Rate Match Pattern1 Bwp Levwl Id bmask = 0
                     Rate Match Pattern2 Cell Level Id bmask = 0
                     Rate Match Pattern2 Bwp Levwl Id bmask = 0
                     Num Prb Bundling
                        Prb Bundling Type = 0
                        Static Bundle Size = 1
                        Dyncamic Bundle Size Set1 = 0
                        Dyncamic Bundle Size Set2 = 0
                     Dmrs Dl Type A[0]
                        Enable = 1
                        Max Length = 0
                        CFG Mask = MASK_SCR0_DEFAULT | MASK_SCR1_DEFAULT
                        Dmrs Type = 0
                        Dmrs Pos = 2
                        Phase Tracking Rs
                           Enable = 0
                           Rsc Element Offeset = 0
                           Epre Ratio = 0
                           CFG Mask = 0
                           Freq Density = { 0, 0 }
                           Time Density = { 0, 0, 0 }
            }
            UL BWP Addmod
               -------------------------------------------------
               |   |          |          |Sub       |          |
               |   |          |          |Carrier   |Cyclic    |
               |#  |BWP Id    |Loc And BW|Spacing   |Prefix    |
               -------------------------------------------------
               |  0|         0|      1099|     30KHZ|    NORMAL|

            Coreset Add Mod
               --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
               |   |          |          |               |                             |                             |                  |          |                    |CCE Req Mapping                                                                        |
               |   |Control   |          |               |                             |                             |                  |          |                    |                                |Interleaved_CCE_Req_Mapping                           |
               |   |Resource  |          |               |                             |                             |                  |Pdcch Dmrs|                    |                                |Req Bundle|                    |InterLeaver|Shift     |
               |#  |Set ID    |Duration  |Freq_Dom_Rsc   |TCI_States_Pdcch_To_Add_Bmask|TCI_States_Pdcch_To_Rel_Bmask|TCI_Present_in_DCI|Scr ID    |Precoder Gran       |CCE_Reg_Mapping_type            |Size      |Precoder_Gran       |Rows       |Index     |
               --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
               |  0|         0|         2|00001E0000000000|             0000000000000000|             0000000000000000|                 0|       186|  SAME_AS_REG_BUNDLE|                     INTERLEAVED|        N6|  SAME_AS_REG_BUNDLE|         N2|     65535|
               |  1|         1|         2|00001FFFFFFFFFFF|             0000000000000000|             0000000000000000|                 0|       186|  SAME_AS_REG_BUNDLE|                 NON_INTERLEAVED|         0|  SAME_AS_REG_BUNDLE|         N2|         0|

            Search Space Add Mod[0] {
               Search Space Id = 0
               CFG Mask = MON_SLT_PERIOD | MON_SYM_IN_SLT | NR_OF_CANDIDATES | SSPACE INFO
               Mon Slot Period = SLOT INVALID
               Control Resource Set Id = 0
               Mon Slot offeset = 0
            }
            Search Space Add Mod[1] {
               Search Space Id = 1
               CFG Mask = MON_SLT_PERIOD | MON_SYM_IN_SLT | NR_OF_CANDIDATES | SSPACE INFO
               Mon Slot Period = 1
               Control Resource Set Id = 0
               Mon Slot offeset = 0
            }
```
## Example Output
```
Active_gNBs = ( "du-rfsim");
# Asn1_verbosity, choice in: none, info, annoying
Asn1_verbosity = "none";

gNBs =
(
 {
    ////////// Identification parameters:
    gNB_ID = 0xe00;
    gNB_DU_ID = 0xe00;
    gNB_name  =  "du-rfsim";

    // Tracking area code, 0x0000 and 0xfffe are reserved values
    tracking_area_code  =  1;
    plmn_list = ({ mcc = 001; mnc = 01; mnc_length = 2; snssaiList = ({ sst = 1; }) });

    nr_cellid = 647169L;

    ////////// Physical parameters:

    min_rxtxtime = 6;

    servingCellConfigCommon = (
    {
 #spCellConfigCommon

      physCellId                                               = 186;

#  downlinkConfigCommon
    #frequencyInfoDL
      # this is the SSB frequency
      absoluteFrequencySSB                                      = 720288;
      dl_frequencyBand                                          = 79;
      # this is the Point A frequency
      dl_absoluteFrequencyPointA                                = 720048;
      #scs-SpecificCarrierList
        dl_offstToCarrier                                       = 0;
# subcarrierSpacing
# 0=kHz15, 1=kHz30, 2=kHz60, 3=kHz120
        dl_subcarrierSpacing                                    = 1;
        dl_carrierBandwidth                                     = 273;
     #initialDownlinkBWP
      #genericParameters
        # this is RBstart=27,L=48 (275*(L-1))+RBstart
        initialDLBWPlocationAndBandwidth                         = 1099; # 6366 12925 12956 28875 12952
# subcarrierSpacing
# 0=kHz15, 1=kHz30, 2=kHz60, 3=kHz120
        initialDLBWPsubcarrierSpacing                             = 1;
      #pdcch-ConfigCommon
        initialDLBWPcontrolResourceSetZero                        = 0;
        initialDLBWPsearchSpaceZero                               = 0;

  #uplinkConfigCommon
     #frequencyInfoUL
      ul_frequencyBand                                             = 79;
      #scs-SpecificCarrierList
      ul_offstToCarrier                                            = 0;
# subcarrierSpacing
# 0=kHz15, 1=kHz30, 2=kHz60, 3=kHz120
      ul_subcarrierSpacing                                         = 1;
      ul_carrierBandwidth                                          = 273;
      pMax                                                         = 23;
     #initialUplinkBWP
      #genericParameters
        initialULBWPlocationAndBandwidth                           = 1099;
# subcarrierSpacing
# 0=kHz15, 1=kHz30, 2=kHz60, 3=kHz120
        initialULBWPsubcarrierSpacing                              = 1;
      #rach-ConfigCommon
        #rach-ConfigGeneric
          prach_ConfigurationIndex                                 = 198;
#prach_msg1_FDM
#0 = one, 1=two, 2=four, 3=eight
          prach_msg1_FDM                                           = 0;
          prach_msg1_FrequencyStart                                = 2;
          zeroCorrelationZoneConfig                                = 10;
          preambleReceivedTargetPower                              = -90;
#preamblTransMax (0...10) = (3,4,5,6,7,8,10,20,50,100,200)
          preambleTransMax                                         = 7;
#powerRampingStep
# 0=dB0,1=dB2,2=dB4,3=dB6
        powerRampingStep                                           = 2;
#ssb_perRACH_OccasionAndCB_PreamblesPerSSB_PR
#1=oneeighth,2=onefourth,3=half,4=one,5=two,6=four,7=eight,8=sixteen
        ssb_perRACH_OccasionAndCB_PreamblesPerSSB_PR               = 4;
#one (0..15) 4,8,12,16,...60,64
        ssb_perRACH_OccasionAndCB_PreamblesPerSSB                  = 32;
#ra_ContentionResolutionTimer
#(0..7) 8,16,24,32,40,48,56,64
        ra_ContentionResolutionTimer                               = 7;
        rsrp_ThresholdSSB                                          = 0;
#prach-RootSequenceIndex_PR
#1 = 839, 2 = 139
        prach_RootSequenceIndex_PR                                 = 2;
        prach_RootSequenceIndex                                    = 4;
        # SCS for msg1, can only be 15 for 30 kHz < 6 GHz, takes precendence over the one derived from prach-ConfigIndex
        #
        msg1_SubcarrierSpacing                                     = 1,
# restrictedSetConfig
# 0=unrestricted, 1=restricted type A, 2=restricted type B
        restrictedSetConfig                                        = 0,

        msg3_DeltaPreamble                                         = 0;
        p0_NominalWithGrant                                        =-78;

# pucch-ConfigCommon setup :
# pucchGroupHopping
# 0 = neither, 1= group hopping, 2=sequence hopping
        pucchGroupHopping                                          = 0;
        hoppingId                                                  = 40;
        p0_nominal                                                 = -96;

      ssb_PositionsInBurst_Bitmap                                  = 128;

# ssb_periodicityServingCell
# 0 = ms5, 1=ms10, 2=ms20, 3=ms40, 4=ms80, 5=ms160, 6=spare2, 7=spare1
      ssb_periodicityServingCell                                   = 2;

# dmrs_TypeA_position
# 0 = pos2, 1 = pos3
      dmrs_TypeA_Position                                           = 0;

# subcarrierSpacing
# 0=kHz15, 1=kHz30, 2=kHz60, 3=kHz120
      subcarrierSpacing                                            = 1;

  #tdd-UL-DL-ConfigurationCommon
# subcarrierSpacing
# 0=kHz15, 1=kHz30, 2=kHz60, 3=kHz120
      referenceSubcarrierSpacing                                   = 1;

      # pattern1
      # dl_UL_TransmissionPeriodicity
      # 0=ms0p5, 1=ms0p625, 2=ms1, 3=ms1p25, 4=ms2, 5=ms2p5, 6=ms5, 7=ms10
      # ext: 8=ms3, 9=ms4
      dl_UL_TransmissionPeriodicity                                = 5;
      nrofDownlinkSlots                                            = 3;
      nrofDownlinkSymbols                                          = 6;
      nrofUplinkSlots                                              = 2;
      nrofUplinkSymbols                                            = 4;

      # pattern2
      pattern2: {
        dl_UL_TransmissionPeriodicity2                             = 4;
        nrofDownlinkSlots2                                         = 4;
        nrofDownlinkSymbols2                                       = 0;
        nrofUplinkSlots2                                           = 0;
        nrofUplinkSymbols2                                         = 0;
      };

      ssPBCH_BlockPower                                            = -11;
     }

  );

    # ------- SCTP definitions
    SCTP :
    {
        # Number of streams to use in input/output
        SCTP_INSTREAMS  = 2;
        SCTP_OUTSTREAMS = 2;
    };
  }
);

MACRLCs = ({
    num_cc              = 1;
    tr_s_preference     = "local_L1";
    tr_n_preference     = "f1";
    local_n_address     = "127.0.0.4";
    remote_n_address    = "127.0.0.3";
    local_n_portd       = 2152;
    remote_n_portd      = 2152;
    pusch_FailureThres  = 1000;
});

L1s = ({
    num_cc = 1;
    tr_n_preference = "local_mac";
    prach_dtx_threshold = 200;
    pucch0_dtx_threshold = 150;
    ofdm_offset_divisor = 8; #set this to UINT_MAX for offset 0
});

RUs = ({
    local_rf       = "yes"
    nb_tx          = 1
    nb_rx          = 1
    att_tx         = 0
    att_rx         = 0;
    bands          = [79];
    max_pdschReferenceSignalPower = -27;
    max_rxgain                    = 114;
    eNB_instances  = [0];
    clock_src = "internal";
});

rfsimulator: {
  serveraddr = "server";
  serverport = 4043;
  options = (); #("saviq"); or/and "chanmod"
  modelname = "AWGN";
  IQfile = "/tmp/rfsimulator.iqs"
}

log_config: {
  global_log_level = "info";
  hw_log_level     = "info";
  nr_phy_log_level = "info";
  nr_mac_log_level = "info";
  rlc_log_level    = "info";
  pdcp_log_level   = "info";
  rrc_log_level    = "info";
  f1ap_log_level   = "info";
  ngap_log_level   = "debug";
};

e2_agent = {
  near_ric_ip_addr = "127.0.0.1";
  sm_dir = "/usr/local/lib/flexric/"
};
```