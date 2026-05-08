project(GD32F5HCP_START LANGUAGES C CXX ASM)

add_library(GD32F5HCP_START OBJECT
    ${DRIVERS_DIR}/BSP/GD32F5HCP_START/gd32f5hcp_start.c
    )

target_include_directories(GD32F5HCP_START PUBLIC
    ${DRIVERS_DIR}/BSP/GD32F5HCP_START
    )

target_link_libraries(GD32F5HCP_START PUBLIC GD32W51x_F5HC_standard_peripheral)
