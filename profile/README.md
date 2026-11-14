<p align="center">
  <img src="https://raw.githubusercontent.com/code-alchemica/.github/main/profile/logo.png" width="120" alt="code-alchemica logo: a flask filled with &lt;/&gt;">
</p>

<h1 align="center">code-alchemica</h1>

<p align="center">Small, sharp developer tools, distilled from real problems.</p>

## Projects

| Project | What it does |
| --- | --- |
| [**hotswap**](https://github.com/code-alchemica/hotswap) | Replace Go functions, methods and variables at run time, in tests. Works natively on Apple silicon. |

```go
hotswap.PatchT(t, time.Now, func() time.Time {
	return time.Date(2026, 8, 17, 9, 0, 0, 0, time.UTC)
})
// Every caller of time.Now, in any package, now gets that date until the test ends.
```

```sh
go get github.com/code-alchemica/hotswap
```
