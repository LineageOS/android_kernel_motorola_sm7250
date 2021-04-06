obj-$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI) += focaltech_0flash_mmi.o
focaltech_0flash_mmi-objs += focaltech_core.o
focaltech_0flash_mmi-objs += focaltech_esdcheck.o
focaltech_0flash_mmi-objs += focaltech_ex_fun.o
focaltech_0flash_mmi-objs += focaltech_ex_mode.o
focaltech_0flash_mmi-objs += focaltech_flash.o
focaltech_0flash_mmi-objs += focaltech_gesture.o
focaltech_0flash_mmi-objs += focaltech_point_report_check.o
focaltech_0flash_mmi-objs += focaltech_test/focaltech_test.o
focaltech_0flash_mmi-objs += focaltech_test/focaltech_test_ini.o

ifneq ($(filter m y,$(CONFIG_INPUT_FOCALTECH_0FLASH_MMI_IC_NAME_FT8719)),)
	ccflags-y += -DCONFIG_INPUT_FOCALTECH_0FLASH_MMI_IC_NAME_FT8719
	focaltech_0flash_mmi-objs += focaltech_test/supported_ic/focaltech_test_ft8719.o
	focaltech_0flash_mmi-objs += focaltech_flash_ft8719.o
	focaltech_0flash_mmi-objs += focaltech_spi_v1_1.o
endif
ifneq ($(filter m y,$(CONFIG_INPUT_FOCALTECH_0FLASH_MMI_IC_NAME_FT8756)),)
	ccflags-y += -DCONFIG_INPUT_FOCALTECH_0FLASH_MMI_IC_NAME_FT8756
	focaltech_0flash_mmi-objs += focaltech_test/supported_ic/focaltech_test_ft8756.o
	focaltech_0flash_mmi-objs += focaltech_flash_ft8756.o
	focaltech_0flash_mmi-objs += focaltech_spi_v1_1_1.o
endif
ifneq ($(filter m y,$(CONFIG_INPUT_FOCALTECH_0FLASH_MMI_IC_NAME_FT8006S_AA)),)
	ccflags-y += -DCONFIG_INPUT_FOCALTECH_0FLASH_MMI_IC_NAME_FT8006S_AA
	ccflags-y += -DFOCALTECH_ESD_EN
	focaltech_0flash_mmi-objs += focaltech_test/supported_ic/focaltech_test_ft8006sp.o
	focaltech_0flash_mmi-objs += focaltech_flash_ft8006s.o
	focaltech_0flash_mmi-objs += focaltech_spi_v1_1_1.o
endif
ifneq ($(filter m y,$(CONFIG_INPUT_FOCALTECH_0FLASH_MMI_IC_NAME_FT8009)),)
	ccflags-y += -DCONFIG_INPUT_FOCALTECH_0FLASH_MMI_IC_NAME_FT8009
	focaltech_0flash_mmi-objs += focaltech_test/supported_ic/focaltech_test_ft8756.o
	focaltech_0flash_mmi-objs += focaltech_flash_ft8756.o
	focaltech_0flash_mmi-objs += focaltech_spi_v1_1_1.o
endif
ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_MMI)),)
       ccflags-y += -DCONFIG_INPUT_TOUCHSCREEN_MMI
       focaltech_0flash_mmi-objs += focaltech_ts_mmi.o
endif
ifneq ($(filter m y,$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI_ENABLE_DOUBLE_TAP)),)
	ccflags-y += -DFOCALTECH_SENSOR_EN
endif
ifneq ($(filter m y,$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI_ENABLE_PALM)),)
	ccflags-y += -DFOCALTECH_PALM_SENSOR_EN
endif
ifneq ($(filter m y,$(CONFIG_TOUCHSCREEN_FTS_0FLASH_MMI_PEN_NOTIFIER)),)
	ccflags-y += -DFOCALTECH_PEN_NOTIFIER
endif
