cmake_minimum_required (VERSION 2.6)
project (CVTree)

ADD_SUBDIRECTORY(src)

INSTALL(DIRECTORY scripts/ DESTINATION bin
  PATTERN "scripts/*"
  PERMISSIONS OWNER_EXECUTE OWNER_WRITE OWNER_READ
              GROUP_EXECUTE GROUP_READ
              WORLD_EXECUTE WORLD_READ )

#INSTALL(FILES COPYRIGHT README DESTINATION share/doc/cvtree)
#INSTALL(DIRECTORY doc/ DESTINATION share/doc/cvtree)
