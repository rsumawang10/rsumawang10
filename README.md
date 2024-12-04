- 👋 Hi, I’m @rsumawang10
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
rsumawang10/rsumawang10 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->@Composable
fun MyApp(
    windowSizeClass: WindowSizeClass = currentWindowAdaptiveInfo().windowSizeClass
) {
    // Perform logic on the size class to decide whether to show the top app bar.
    val showTopAppBar = windowSizeClass.windowHeightSizeClass != WindowHeightSizeClass.COMPACT

    // MyScreen knows nothing about window sizes, and performs logic based on a Boolean flag.
    MyScreen(
        showTopAppBar = showTopAppBar,
        /* ... */
    )
}
