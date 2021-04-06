ifneq ($(filter m y, $(CONFIG_PANEL_NOTIFICATIONS)),)
	ccflags-y += -DCONFIG_PANEL_NOTIFICATIONS
endif

ifneq ($(filter m y, $(CONFIG_DRM_DYNAMIC_REFRESH_RATE)),)
	ccflags -y += -DCONFIG_DRM_DYNAMIC_REFRESH_RATE
endif

ifneq ($(filter m y, $(CONFIG_TOUCHCLASS_MMI_DEBUG_INFO)),)
	ccflags-y += -DCONFIG_TOUCHCLASS_MMI_DEBUG_INFO
endif

ifneq ($(filter m y, $(CONFIG_TOUCHCLASS_MMI_GESTURE_POISON_EVENT)),)
	ccflags-y += -DTS_MMI_TOUCH_GESTURE_POISON_EVENT
endif

ifneq ($(filter m y, $(CONFIG_DRM_PANEL_NOTIFICATIONS)),)
	ccflags-y += -DCONFIG_DRM_PANEL_NOTIFICATIONS
endif

touchscreen_mmi-y += touchscreen_mmi_class.o touchscreen_mmi_panel.o touchscreen_mmi_notif.o touchscreen_mmi_gesture.o

obj-$(CONFIG_INPUT_TOUCHSCREEN_MMI) += touchscreen_mmi.o
