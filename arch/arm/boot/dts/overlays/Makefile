ifeq ($(CONFIG_OF),y)

# Overlays for the AEMICS DIN module platform
ifeq ($(CONFIG_SOC_SAM_V7),y)
   AEDIN_DT_OVERLAYS=y
endif

dtbo-$(AEDIN_DT_OVERLAYS) += flx2_uart.dtbo
dtbo-$(AEDIN_DT_OVERLAYS) += flx2_spi.dtbo
dtbo-$(AEDIN_DT_OVERLAYS) += flx2_i2c.dtbo
dtbo-$(AEDIN_DT_OVERLAYS) += flx3_uart.dtbo
dtbo-$(AEDIN_DT_OVERLAYS) += flx3_spi.dtbo
dtbo-$(AEDIN_DT_OVERLAYS) += flx3_i2c.dtbo

dtbo-$(AEDIN_DT_OVERLAYS) += flx2_spi_eeprom.dtbo
dtbo-$(AEDIN_DT_OVERLAYS) += flx3_spi_eeprom.dtbo

targets += dtbs dtbs_install
targets += $(dtbo-y)

endif

always		:= $(dtbo-y)
clean-files	:= *.dtbo
