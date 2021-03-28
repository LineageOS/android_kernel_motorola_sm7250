#
# Makefile for the Trustonic core driver
#

GUD_ROOT_FOLDER := drivers/gud/

ifneq ($(filter m y,$(CONFIG_TRUSTONIC_TEE_DEBUG)),)
	ccflags-y += -DDEBUG
endif

ifneq ($(filter m y,$(CONFIG_RSU_SELECT_SILVER_CORES)),)
	ccflags-y += -DRSU_SELECT_SILVER_CORES
endif

ifneq ($(filter m y,$(CONFIG_RSU_INTERNAL_CLOCK)),)
	ccflags-y += -DRSU_INTERNAL_CLOCK
endif

obj-$(CONFIG_TRUSTONIC_TEE) += mcDrvModule.o

mcDrvModule-y := \
	admin.o \
	client.o \
	clientlib.o \
	clock.o \
	fastcall.o \
	iwp.o \
	logging.o \
	main.o \
	mcp.o \
	mmu.o \
	nq.o \
	session.o \
	teeclientapi.o \
	user.o \
	xen_be.o \
	xen_common.o \
	xen_fe.o

# MobiCore Driver includes
ccflags-y += -I$(GUD_ROOT_FOLDER)/MobiCoreDriver
