Orbit — Virtual File System and Command Dispatch Engine
Orbit is a C++17 systems-programming project that implements an in-memory virtual file system, a command-line interface and a small command-dispatch layer. The project is intended as a learning and engineering exercise in ownership, tree data structures, command parsing, persistence and modular C++ design.
Features
• In-memory N-ary file and directory tree.
• Ownership of child nodes through std::unique_ptr.
• Navigation commands such as cd, pwd, ls and tree.
• File and directory manipulation commands including mkdir, rm, cp and wtf.
• Recursive search and content search.
• Favorite/write-protection flags.
• Binary save/load support for the current file-system state.
• A command dispatcher generated from an X-macro command list.
• A small .orb scripting prototype.
• A diagnostic command test runner.
Build and run
On a Linux environment with a C++17 compiler:
shell
make run
Use code with caution.
Run the diagnostic suite
shell
make test
Use code with caution.
The current test runner executes a scripted set of commands and reports command-level failures. It is a smoke-test suite rather than a complete unit, property-based or fuzz-testing framework.
