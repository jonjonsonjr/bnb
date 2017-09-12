# Life is hard

	$ blaze run :hello_world_image                                                                                                                                                                           (master✱)
	...........
	ERROR: /Users/jon/projects/repro/src/BUILD:9:1: every rule of type go_binary implicitly depends upon the target '//:go_prefix', but this target could not be found because of: no such package '': BUILD file not found on package path.
	ERROR: Analysis of target '//src:hello_world_image' failed; build aborted.
	INFO: Elapsed time: 7.743s
	ERROR: Build failed. Not running target.
