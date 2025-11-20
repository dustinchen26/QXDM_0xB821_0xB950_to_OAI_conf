# QXDM_0xB821_0xB950_to_OAI_conf

online calculator: https://dustinchen26.github.io/QXDM_0xB821_0xB950_to_OAI_conf

## How to use
```
把QXDM[0xB821][0xB950]複製貼到輸入框，即可解析出OAI conf，記得QXDM Options->Export Parsed Text
(PS) cedar要修改滿足OAI，不然會Assertion (prach_info.start_symbol + prach_info.N_t_slot * prach_info.N_dur < 14                                                                                               ) failed!
prach_ConfigurationIndex = 147; #把147改成75
```

## Example Input
```
20:45:29.807326          OTA LOG                  [0xB821]                 BCCH_DL_SCH / SystemInformationBlockType1                   BCCH_DL_SCH / SystemInformationBlockType1
20:45:29.807326
20:45:29.807326	[0xB821]	BCCH_DL_SCH / SystemInformationBlockType1
Pkt Version = 9
RRC Release Number.Major.minor = 15.9.0
Radio Bearer ID = 0, Physical Cell ID = 186
NR Cell Global Id = N/A
Freq = 644736
Sfn = 608, SubFrameNum = 0
slot = 0
PDU Number = BCCH_DL_SCH Message,    Msg Length = 123
SIB Mask in SI =  0x02

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
          plmn-IdentityList 
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
                  freqBandIndicatorNR 78
                }
              },
              offsetToPointA 24,
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
                  controlResourceSetZero 10,
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
                      startSymbolAndLength 40
                    },
                    {
                      mappingType typeA,
                      startSymbolAndLength 96
                    },
                    {
                      mappingType typeA,
                      startSymbolAndLength 68
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
              firstPDCCH-MonitoringOccasionOfPO sCS120KHZquarterT-SCS60KHZoneEighthT-SCS30KHZoneSixteenthT : 
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
                    prach-ConfigurationIndex 147,
                    msg1-FDM one,
                    msg1-FrequencyStart 2,
                    zeroCorrelationZoneConfig 10,
                    preambleReceivedTargetPower -90,
                    preambleTransMax n6,
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
                  p0-NominalWithGrant -96
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
              nrofDownlinkSymbols 10,
              nrofUplinkSlots 1,
              nrofUplinkSymbols 2
            },
            pattern2 
            {
              dl-UL-TransmissionPeriodicity ms2p5,
              nrofDownlinkSlots 2,
              nrofDownlinkSymbols 10,
              nrofUplinkSlots 2,
              nrofUplinkSymbols 2
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
20:45:29.812033          LOG                      [0xB950]                 NR5G ML1 DL Common Config                                   Length:   52
20:45:29.812033
20:45:29.812033	[0xB950]	NR5G ML1 DL Common Config
Major.Minor Version = 2. 6
ota_cfg_param
   logging_time_sub_fn = 7
   logging_time_sys_fn = 572
   num_cg_add_mod = 1
   cg_add_mod
      log_mask = 0b
      common_cg_cfg
         cell_group_id = 0
         target_dl_cell_frequency = 644736
         target_phy_cell_id = 186
         cfg_mask = MAIN
         cc_id_del_bmask = 00000000b
         cc_id_addmod_bmask = 00000001b
         rlm_in_sync_out_of_sync_threshold = 0
         mac_main_cfg {
            is_cdrx_config_present = 0
            reserved = 0
         }
20:45:29.812071          LOG                      [0xB950]                 NR5G ML1 DL Common Config                                   Length:  636
20:45:29.812071
20:45:29.812071	[0xB950]	NR5G ML1 DL Common Config
Major.Minor Version = 2. 6
ota_cfg_param
   logging_time_sub_fn = 7
   logging_time_sys_fn = 572
   num_cg_add_mod = 1
   cg_add_mod
      log_mask = 1b
      per_cc_cfg
         cell_info
            band = SYS_SBAND_NR5G_BAND78
            phy_cell_id = 186
            ssb_sub_carrier_spacing = SSB_30KHZ
            dl_cell_frequency = 644736
         duplex_mode = TDD
         scc_id = 0
         serv_cell_idx = 0
         num_coreset_add_mod = 2
         num_search_space_add_mod = 2
         num_dl_bwp_id_addmod = 1
         num_ul_bwp_id_addmod = 1
         dl_bwp_id_rel_bmask = 00000000b
         dl_bwp_id_addmod_bmask = 00000001b
         ul_bwp_id_rel_bmask = 00000000b
         ul_bwp_id_addmod_bmask = 00000001b
         cfg_mask = COMMON | DEDICATED | DL_FREQ_INFO | UL_FREQ_INFO
         cc_com_cfg[0]
            dmrs_type_a_pos = NR5G_DL_DMRS_ADD_POS_2
            ss_pbch_blk_pwr = -11
            ssb_period = NR5G_SSB_PERIODICITY_SERV_CELL_MS20
            rate_match_pattern_id_rel_bmask = 0
            rate_match_pattern_addmod_bmask = 0
            cfg_mask = SSB_POS_BURST | SUB_CAR_SPACING | TDD_UL_DL | 0x10
            sub_carr_spacing = NR5G_COMMON_SUB_CARR_SPACING_kHz30
            ssb_pos_in_burst_bmask = 0x8000000000000000
            tdd_ul_dl_cfg_common[0]
               enable = 1
               ref_scs = 1
               pattern2_enable = 1
               pattern1
                  dl_ul_trans_period = MS2_5
                  num_dl_sym = 10
                  num_ul_sym = 2
                  num_dl_slots = 3
                  num_ul_slots = 1
               pattern2
                  dl_ul_trans_period = MS2_5
                  num_dl_sym = 10
                  num_ul_sym = 2
                  num_dl_slots = 2
                  num_ul_slots = 2
         cc_ded_cfg[0] {
            tag_id = 0
            bwp_inact_timer = MS0
            first_active_dl_bwp_id = 0
            default_dl_bwp_id = 0
            first_active_ul_bwp = 0
            ue_beam_lock_fn = 0
            serving_cell_mo_id = 255
            cfg_mask =                         0
            path_loss_reference_linking = PCELL
            antenna_info_dl {
               max_mimo_lyr_cfged = 1
               max_num_mimo_lyr = LAYER_FOUR
               max_num_rx = FOUR
            }
         }
         dl_freq_info[0]
            abs_freq_ssb = 644736
            abs_freq_point_a = 644208
            num_scs_carriers = 1
            multi_freq_band_list
               num_bands = 1
               freq_band_indicator = { 78, 0, 0, 0, 0, 0, 0, 0 }
            scs_spec_carr_list
               ----------------------------------------------------------------
               |#  |offset_to_carr|carrier_bw_prb|scs         |carrier_bw     |
               ----------------------------------------------------------------
               |  0|             0|           273|       kHz30| NR5G_BW_200MHz|
               |  1|             0|             0|       kHz15|   NR5G_BW_5MHz|
               |  2|             0|             0|       kHz15|   NR5G_BW_5MHz|
               |  3|             0|             0|       kHz15|   NR5G_BW_5MHz|
               |  4|             0|             0|       kHz15|   NR5G_BW_5MHz|

         ul_freq_info[0]
            abs_freq_point_a = 644208
            p_max = 230
            add_spectrum_emission_present = 0
            add_spectrum_emission = 0
            freq_shift_7p5_khz = 0
            num_scs_carriers = 1
            multi_freq_band_list
               num_bands = 1
               freq_band_indicator = { 78, 0, 0, 0, 0, 0, 0, 0 }
            scs_spec_carr_list
               ----------------------------------------------------------------
               |#  |offset_to_carr|carrier_bw_prb|scs         |carrier_bw     |
               ----------------------------------------------------------------
               |  0|             0|           273|       kHz30| NR5G_BW_200MHz|
               |  1|             0|             0|       kHz15|   NR5G_BW_5MHz|
               |  2|             0|             0|       kHz15|   NR5G_BW_5MHz|
               |  3|             0|             0|       kHz15|   NR5G_BW_5MHz|
               |  4|             0|             0|       kHz15|   NR5G_BW_5MHz|

         dl_bwp_params[0]
            bwp_generic_params
               bwp_id = 0
               loc_and_bw = 1099
               sub_carr_spacing = kHz30
               cyclic_prefix = NORMAL
            cfg_mask = COMMON | DEDICATED
            dl_bwp_common[0]
               cfg_mask = PDCCH | PDSCH
               pdcch_common[0]
                  enable = 1
                  corset_zero_id = 10
                  searchspace_zero_id = 0
                  coreset_active_bmask = 1
                  coreset_rel_bmask = 0
                  search_space_active_bmask = 0x0000000000000003
                  search_space_rel_bmask = 0x0000000000000000
                  search_space_id_RMSI = 0
                  search_space_id_OSI = 1
                  search_space_id_paging = 1
                  search_space_id_ra = 1
               pdsch_common[0]
                  enable = 1
                  num_pdsch_alloc_list = 3
                  pdsch_time_dom_alloc_list
                     -----------------------------------------------------
                     |#  |k_present|mapping_type|k  |start_sum_and_length|
                     -----------------------------------------------------
                     |  0|        0|      TYPE_A|  0|                  40|
                     |  1|        0|      TYPE_A|  0|                  96|
                     |  2|        0|      TYPE_A|  0|                  68|
                     |  3|        0|      TYPE_A|  0|                   0|
                     |  4|        0|      TYPE_A|  0|                   0|
                     |  5|        0|      TYPE_A|  0|                   0|
                     |  6|        0|      TYPE_A|  0|                   0|
                     |  7|        0|      TYPE_A|  0|                   0|
                     |  8|        0|      TYPE_A|  0|                   0|
                     |  9|        0|      TYPE_A|  0|                   0|
                     | 10|        0|      TYPE_A|  0|                   0|
                     | 11|        0|      TYPE_A|  0|                   0|
                     | 12|        0|      TYPE_A|  0|                   0|
                     | 13|        0|      TYPE_A|  0|                   0|
                     | 14|        0|      TYPE_A|  0|                   0|
                     | 15|        0|      TYPE_A|  0|                   0|

            dl_bwp_ded[0]
               cfg_mask = PDSCH
               pdsch_cfg_ded[0]
                  enable = 1
                  mcs_table = MCS_256QAM
                  rbg_size = 1
                  cfg_mask = DATA_SCR_ID | DMRS_DL_TYPEA
                  pdsch_rsc_alloc = RATP1
                  max_code_words_scheduled_by_dci = N1
                  vrb_to_prb_interleaver = NONE
                  data_scr_id = 65535
                  num_pdsch_alloc_list = 0
                  prb_bundling
                     prb_bundling_type = 0
                     static_BundleSize = 1
                     dynamic_BundleSize_set1 = 0
                     dynamic_BundleSize_set2 = 0
                  dmrs_dl_typeA[0]
                     enable = 1
                     max_length = 0
                     cfg_mask = SCR0_DEFAULT | SCR1_DEFAULT
                     dmrs_type = 0
                     dmrs_pos = 2
                     dmrs_scr_id0 = 65535
                     dmrs_scr_id1 = 65535
                     phase_tracking_rs
                        enable = 0
                        rsc_element_offset = 0
                        epre_ratio = 0
                        cfg_mask = 0
                        freq_density = { 0, 0 }
                        time_density = { 0, 0, 0 }
         ul_bwp_addmod
            ------------------------------------------------------
            |#  |bwp_id|loc_and_bw|sub_carr_spacing|cyclic_prefix|
            ------------------------------------------------------
            |  0|     0|      1099|           kHz30|       NORMAL|

         coreset_add_mod
            --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
            |   |                       |        |            |                            |                            |                  |                 |                    |cce_reg_mapping                                                                       |
            |   |                       |        |            |                            |                            |                  |                 |                    |                    |interleaved_cce_reg_mapping                                      |
            |#  |control_resource_set_id|duration|freq_dom_rsc|tci_states_pdcch_to_add_bmsk|tci_states_pdcch_to_rel_bmsk|tci_present_in_dci|pdcch_dmrs_scr_id|precoder_gran       |cce_reg_mapping_type|reg_bundle_size|precoder_gran       |interleaver_rows|shift_index|
            --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
            |  0|                      0|       1|35046933135360|          0x0000000000000000|          0x0000000000000000|                 0|              186|  SAME_AS_REG_BUNDLE|                   0|             N6|  SAME_AS_REG_BUNDLE|              N2|      65535|
            |  1|                      1|       1|35184372088831|          0x0000000000000000|          0x0000000000000000|                 0|              186|  SAME_AS_REG_BUNDLE|                   1|              0|  SAME_AS_REG_BUNDLE|              N2|          0|

         search_space_add_mod[0]
            search_space_id = 0
            num_candidates_aggr_level
               aggr_level_1 = N0
               aggr_level_2 = N0
               aggr_level_4 = N4
               aggr_level_8 = N2
               aggr_level_16 = N1
            cfg_mask = MON_SLT_PERIOD | MON_SYM_IN_SLT | NR_OF_CANDIDATES | SSPACE_INFO
            mon_slot_period = INVALID
            control_resource_set_id = 0
            mon_slot_offset = 0
            mon_sym_within_slot_bmask = 0010000000000000b
            search_space
               sspace_type = COMMON
               common_sspace
                  cfg_mask = FMT_00_10 | FMT_20_RELEASE | FMT_21_RELEASE | FMT_22_RELEASE | FMT_23_RELEASE
                  format_00_and_format_10
                     temp = 0
                  format_20
                     aggr_level_is_valid = 0
                     nr_of_candidates_sfi
                        aggr_level_1 = N0
                        aggr_level_2 = N0
                        aggr_level_4 = N0
                        aggr_level_8 = N0
                        aggr_level_16 = N0
                  format_21
                     temp = 0
                  format_22
                     temp = 0
                  format_23
                     mon_period = INVALID
                     num_pdcch_cand = N1
         search_space_add_mod[1]
            search_space_id = 1
            num_candidates_aggr_level
               aggr_level_1 = N0
               aggr_level_2 = N0
               aggr_level_4 = N4
               aggr_level_8 = N2
               aggr_level_16 = N1
            cfg_mask = MON_SLT_PERIOD | MON_SYM_IN_SLT | NR_OF_CANDIDATES | SSPACE_INFO
            mon_slot_period = N1
            control_resource_set_id = 0
            mon_slot_offset = 0
            mon_sym_within_slot_bmask = 0010000000000000b
            search_space
               sspace_type = COMMON
               common_sspace
                  cfg_mask = FMT_00_10 | FMT_20_RELEASE | FMT_21_RELEASE | FMT_22_RELEASE | FMT_23_RELEASE
                  format_00_and_format_10
                     temp = 0
                  format_20
                     aggr_level_is_valid = 0
                     nr_of_candidates_sfi
                        aggr_level_1 = N0
                        aggr_level_2 = N0
                        aggr_level_4 = N0
                        aggr_level_8 = N0
                        aggr_level_16 = N0
                  format_21
                     temp = 0
                  format_22
                     temp = 0
                  format_23
                     mon_period = INVALID
                     num_pdcch_cand = N1

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
      absoluteFrequencySSB                                      = 644736;
      dl_frequencyBand                                          = 78;
      # this is the Point A frequency
      dl_absoluteFrequencyPointA                                = 644208;
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
        initialDLBWPcontrolResourceSetZero                        = 10;
        initialDLBWPsearchSpaceZero                               = 0;

  #uplinkConfigCommon
     #frequencyInfoUL
      ul_frequencyBand                                             = 78;
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
          prach_ConfigurationIndex                                 = 75; #把147改成75
#prach_msg1_FDM
#0 = one, 1=two, 2=four, 3=eight
          prach_msg1_FDM                                           = 0;
          prach_msg1_FrequencyStart                                = 2;
          zeroCorrelationZoneConfig                                = 10;
          preambleReceivedTargetPower                              = -90;
#preamblTransMax (0...10) = (3,4,5,6,7,8,10,20,50,100,200)
          preambleTransMax                                         = 3;
#powerRampingStep
# 0=dB0,1=dB2,2=dB4,3=dB6
        powerRampingStep                                           = 2;
#ssb_perRACH_OccasionAndCB_PreamblesPerSSB_PR
#1=oneeighth,2=onefourth,3=half,4=one,5=two,6=four,7=eight,8=sixteen
        ssb_perRACH_OccasionAndCB_PreamblesPerSSB_PR               = 4;
#one (0..15) 4,8,12,16,...60,64
        ssb_perRACH_OccasionAndCB_PreamblesPerSSB                  = 7;
#ra_ContentionResolutionTimer
#(0..7) 8,16,24,32,40,48,56,64
        ra_ContentionResolutionTimer                               = 7;
        rsrp_ThresholdSSB                                          = 0;
#prach-RootSequenceIndex_PR
#1 = 839, 2 = 139
        prach_RootSequenceIndex_PR                                 = 2;
        prach_RootSequenceIndex                                    = 1;
        # SCS for msg1, can only be 15 for 30 kHz < 6 GHz, takes precendence over the one derived from prach-ConfigIndex
        #
        msg1_SubcarrierSpacing                                     = 1,
# restrictedSetConfig
# 0=unrestricted, 1=restricted type A, 2=restricted type B
        restrictedSetConfig                                        = 0,

        msg3_DeltaPreamble                                         = 0;
        p0_NominalWithGrant                                        =-96;

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
      nrofDownlinkSymbols                                          = 10;
      nrofUplinkSlots                                              = 1;
      nrofUplinkSymbols                                            = 2;

      # pattern2
      pattern2: {
        dl_UL_TransmissionPeriodicity2                             = 5;
        nrofDownlinkSlots2                                         = 2;
        nrofDownlinkSymbols2                                       = 10;
        nrofUplinkSlots2                                           = 2;
        nrofUplinkSymbols2                                         = 2;
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
    bands          = [78];
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