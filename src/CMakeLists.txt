set(EXTRA_COMPONENT_DIRS lib drivers)

idf_component_register(
    SRCS "*.c"
    INCLUDE_DIRS "." include
    REQUIRES freertos esp_event esp_common esp32_cam
)
