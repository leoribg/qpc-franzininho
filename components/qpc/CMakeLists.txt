
file(GLOB QPC qpc/ports/freertos-esp32/*.c qpc/src/qf/*.c qpc/include/*.c)

idf_component_register(SRCS ${QPC}
                       INCLUDE_DIRS "qpc/include" "qpc/ports/freertos-esp32" "qpc/src"
                       REQUIRES freertos)
