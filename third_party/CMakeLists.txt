#if(JCONF_USE_EXTERNAL_JSON)
  #find_package(nlohmann_json 3.7.0 REQUIRED)
#else()
  #set(JSON_BuildTests OFF CACHE INTERNAL "")
  #add_subdirectory(json)
#endif()

add_subdirectory(JConf)
