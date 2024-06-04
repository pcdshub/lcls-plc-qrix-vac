IOC_TOP=/reg/g/pcds/epics/ioc/common/ads-ioc/R0.6.2
IOC_INSTANCE_PATH := $(shell pwd)

# Set PRODUCTION_IOC to 1 to move from a testing to a production IOC:
PRODUCTION_IOC := 1

PROJECT_NAME := lcls-plc-qrix-vac
PROJECT_PATH := ../../lcls-plc-qrix-vac/lcls-plc-qrix-vac/lcls-plc-qrix-vac.tsproj
PLC := PLC_QRIX_VAC

PYTMC_OPTS := 
PREFIX := PLC:QRIX:VAC

# With two $$, as in $$(IOC) below, this will be expanded in the
# environment of st.cmd:
DB_PARAMETERS := 'PREFIX=$(PREFIX):,IOCNAME=$$(IOC),IOC=$$(IOC)'

include $(IOC_TOP)/iocBoot/templates/Makefile.base
