# Command
Zircon's Executable or Shell Command Execution Module, it, like rest of the Standard Library, follows a context-based approach.

## `ExecutionContext`
```json
ExecutionContext {
	from: String,
	use_native_shell?: Boolean
}
```

An `ExecutionContext` takes in a `from` field, which can be supplied with the name of an executable available in the PATH Environment Variable to work with. If the string is empty, it will pipe to your system shell, which by default is PowerShell on Windows or zsh on macOS. 

```js
context = ExecutionContext with 
	from: ""
end

context.invoke "Write-Output 'Hello, from Zircon!'"
```
The Above Example creates an empty context, which would create a PowerShell instance on Windows. Then, we call `invoke` with a command in string form to execute. On Windows, the command will then write "Hello, from Zircon!" to Standard Output of your Shell/Terminal.