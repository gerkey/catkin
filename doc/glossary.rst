Glossary
--------

.. glossary::

   dry
        a (package/stack/whatever) not yet converted to catkin/FHS build & install.

   wet
        a (package/stack/whatever) stack already converted to catkin/FHS build & install.

   stack
        unit of installation.  These get made in to debs.

   package
        generally something "smaller" than a stack... but a package
        can be a stack.

   project
        CMake's notion of buildable subdirectory: it contains a
        ``CMakeLists.txt`` that calls CMake's ``project()`` macro.  These can next.

   generated code
        Code generated during the build process, typically by a message code generator package.
        May or may not require compilation.

   static code
        Code typed in by a developer, contrast :term:`generated code`

   config-mode infrastructure
        Files named ``<project>-config.cmake`` and
        ``<project>-config-version.cmake`` which are used by cmake's
        ``find_package()`` in "config mode".

   pkgutil
        Nifty python package:
        http://docs.python.org/library/pkgutil.html

   cmake current files directory
        A location used by catkin to store intermediate
        files generated by cmake.  Catkin uses
        ``${CMAKE_CURRENT_FILES_DIRECTORY}${CMAKE_FILES_DIRECTORY}``,
        for instance
        ``... build/ros_comm/clients/cpp/roscpp/CMakeFiles``.  (Note
        the ``CMakeFiles`` at the end of that path)


