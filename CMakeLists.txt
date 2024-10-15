# Copyright (c) 2020 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(LIS2DW12 INTERFACE)

target_include_directories(LIS2DW12
    INTERFACE
        ./
        ./ST_INTERFACES/Communications/
        ./X_NUCLEO_COMMON/DevSPI/
        ./ST_INTERFACES/Sensors/
        ./X_NUCLEO_COMMON/DevI2C/
        ./ST_INTERFACES/Common/
)

target_sources(LIS2DW12
    INTERFACE
        ./LIS2DW12Sensor.cpp
        ./lis2dw12_reg.c
)