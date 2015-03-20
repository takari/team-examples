# Smart Builder

This is an example of how to setup the [Takari Smart Builder][1] along with the [Concurrent Safe Local Repository][2]. Note that you always want to use two extensions together to account for now Maven resolves dependencies on a per-project basis. Two projects that may build in parallel may have the same dependency and if they both request this depedency simultaneously you need to Concurrent Safe Local Repository to synchronize the write to the local repository.

[1]: http://takari.io/book/30-team-maven.html#takari-smart-builder
[2]: http://takari.io/book/30-team-maven.html#concurrent-safe-local-repository
