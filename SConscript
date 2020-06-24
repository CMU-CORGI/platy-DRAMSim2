
import os

env = Environment(ENV = os.environ)
env.Append(CXXFLAGS = ["-DNO_STORAGE", "-Wall", "-DDEBUG_BUILD", "-fabi-version=2", "-D_GLIBCXX_USE_CXX11_ABI=0"])

sources = [x for x in Glob("*.cpp") if str(x) != "TraceBasedSim.cpp"]
dramsim = env.StaticLibrary("dramsim", sources)

Return("dramsim")

