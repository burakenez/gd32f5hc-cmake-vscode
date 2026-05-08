project(GD32F5HCR_EVAL LANGUAGES C CXX ASM)

add_library(GD32F5HCR_EVAL OBJECT
    ${DRIVERS_DIR}/BSP/GD32F5HCR_EVAL/gd32f5hcr_eval.c
    )

target_include_directories(GD32F5HCR_EVAL PUBLIC
    ${DRIVERS_DIR}/BSP/GD32F5HCR_EVAL
    )

target_link_libraries(GD32F5HCR_EVAL PUBLIC GD32W51x_F5HC_standard_peripheral)
