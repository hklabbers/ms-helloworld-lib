set(HEADER_FILES AbstractRequestHandler.h
        MicroServerHelloWorldRequestHandler.h
        MicroServerRequestHandlerProvider.h
        )

set(SOURCE_FILES AbstractRequestHandler.cpp
        MicroServerHelloWorldRequestHandler.cpp
        MicroServerRequestHandlerProvider.cpp
        Manifest.cpp
        )

add_library (ms-helloworld SHARED ${SOURCE_FILES} ${HEADER_FILES} )

target_link_libraries (ms-helloworld LINK_PUBLIC ${POCO} )
