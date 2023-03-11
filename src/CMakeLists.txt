set(COMPONENT_SRCS 
    take_picture.c
    drivers/camera_capture/app_wifi.c
    drivers/camera_capture/stream_server.c
)

set(COMPONENT_ADD_INCLUDEDIRS 
    include/
    drivers/camera_capture/include/
)

set(COMPONENT_REQUIRES
    freertos 
    nvs_flash 
    esp_event 
    esp_common 
    esp_wifi 
    esp32_cam 
    esp_http_server
)

register_component()
