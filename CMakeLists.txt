add_library(canopennode STATIC
    CANopen.c
    OD.c
    
    301/CO_Emergency.c
    301/CO_fifo.c
    301/CO_HBconsumer.c
    301/CO_NMT_Heartbeat.c
    301/CO_Node_Guarding.c
    301/CO_ODinterface.c
    301/CO_PDO.c
    301/CO_SDOclient.c
    301/CO_SDOserver.c
    301/CO_SYNC.c
    301/CO_TIME.c
)

target_include_directories(canopennode PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
    ${CMAKE_CURRENT_SOURCE_DIR}/301
    ${CMAKE_SOURCE_DIR}/inc
)