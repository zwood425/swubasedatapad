idf_component_register(
    SRCS "main.c"
    INCLUDE_DIRS "."
    REQUIRES user_encoder_bsp i2c_bsp lcd_touch_bsp lcd_bl_pwm_bsp i2c_equipment)

set_source_files_properties(
    ${LV_DEMOS_SOURCES}
    PROPERTIES COMPILE_OPTIONS
    -DLV_LVGL_H_INCLUDE_SIMPLE)
