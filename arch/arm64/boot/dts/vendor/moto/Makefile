ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
        dtbo-$(CONFIG_RACER_DTB) += \
                racer/lito-racer_01.dtbo \
                racer/lito-racer_02.dtbo \
                racer/lito-racer_03.dtbo

        dtbo-$(CONFIG_SMITH_DTB) += \
                smith/lito-smith_01.dtbo \
                smith/lito-smith_02.dtbo \
                smith/lito-smith_03.dtbo \
                smith/lito-smith_04.dtbo \
                smith/lito-smith_05.dtbo \
                smith/lito-smith_06.dtbo \
                smith/lito-smith_07.dtbo \
                smith/lito-smith_08.dtbo

		dtbo-$(CONFIG_KIEV_DTB) += \
				kiev/lagoon-kiev_01.dtbo \
				kiev/lagoon-kiev_02.dtbo
endif

always		:= $(dtb-y) $(dtbo-y)
subdir-y	:= $(dts-dirs)
clean-files    := *.dtb *.dtbo
