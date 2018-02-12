# MouseInjectDetection
Simple method of checking whether or not mouse movement or buttons (&lt;windows 10) are injected.
Could be used by anti cheat providers as an easy way to tell if someone is using aim assist.

# Build
Open in visual studio and build

# Use
According to the windows documentation you would want to compile and run x86 and x64 versions to account for all.

# Methods to bypass
Hook and unhook WH_MOUSE_LL and modify the injected flag so other hooks don't see it as injected.
You want your hook to always be the last hook that was set to be the first one called so maybe some sort of periodic unset and set will work well.  