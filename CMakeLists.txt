SET(SOURCES_DIRS "src"
    "src/AsyncMqttClient"
    "src/AsyncMqttClient/Packets"
    "src/AsyncMqttClient/Packets/Out"
)

idf_component_register(SRC_DIRS "${SOURCES_DIRS}"
    INCLUDE_DIRS "${SOURCES_DIRS}"
    REQUIRES arduino AsyncTCP
)
