# networking-ts-merge
Capturing merge criteria for the Networking TS

## Use of dispatch, post and defer

US 10 and the elaboration in <a href="http://wg21.link/p0703r0">P0703R0</a> proposed removing the `defer` function from executors.

"We find the difference between post and defer to be too subtle and too executor-specific to be useful in the C++ standard. The confusion caused outweighs the performance gain in the Bloomberg committee's opinion. Additionally, it has not been demonstrated that performance gains from having a distinction between post and defer make a difference in any real-world applications."

The NB comment was rejected, with 'no consensus for change' 

However the TS should provide opportunity to capture user feedback on this issue:
   * Does the presence of the three methods cause confusion to users?
   * Is there a performance gain (which is not simply an implementation artefact)?
   * Are there other ways to achive a similar aim (eg other changes to the executor model)

