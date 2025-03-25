![TIMISONG's Git Stats](https://github-readme-stats.vercel.app/api?username=timisong-dev&theme=dark&layout=compact)
![Favorite Lang's](https://github-readme-stats.vercel.app/api/top-langs/?username=timisong-dev&theme=dark&layout=compact)


```kotlin
package timisongdev.timisong
        
import ...

class MainActivity : ComponentActivity() {
    @SuppressLint("UnusedMaterial3ScaffoldPaddingParameter")
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        enableEdgeToEdge()
        setContent {
            TimisongTheme {
                Scaffold {
                    Greeting()
                }
            }
        }
    }
}

class MainActivity : ComponentActivity() {
    @SuppressLint("UnusedMaterial3ScaffoldPaddingParameter")
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        enableEdgeToEdge()
        setContent {
            TIMISONGTheme {
                Scaffold {
                    Greeting()
                }
            }
        }
    }
}

@Composable
fun Greeting() {

    val context = LocalContext.current
    Column (
        Modifier
            .padding(8.dp)
            .fillMaxSize(),
        horizontalAlignment = Alignment.CenterHorizontally,
        verticalArrangement = Arrangement.Center
    ) {
        Text (
            "TIMISONG-dev",
            fontSize = 18.sp,
            fontWeight = FontWeight.Bold
        )
        Spacer(
            Modifier
                .padding(16.dp)
        )
        Text (
            "Hello, I'm Dmitry, I'm an android dev, I know the following langs: \n" +
            "Kotlin, Java, Flutter, C#, C++\n" +
            "\n" +
            "I also play guitar and piano as a hobby. Currently working on a kernel for Poco F3 (Kona/Alioth/4.19) ",
        )
        Spacer(
            Modifier
                .padding(16.dp)
        )
        Row (
            verticalAlignment = Alignment.CenterVertically,
            horizontalArrangement = Arrangement.Center
        ) {
            Text (
                "Telegram channel: ",
                fontSize = 16.sp
            )
            Text (
                "t.me/timisong_dev",
                Modifier
                    .clickable{
                        val intent = Intent(Intent.ACTION_VIEW, "https://t.me/timisong_dev".toUri())
                        context.startActivity(intent)
                    },
                color = MaterialTheme.colorScheme.primary,
                textDecoration = TextDecoration.Underline,
                fontSize = 16.sp
            )
        }
        Row (
            verticalAlignment = Alignment.CenterVertically,
            horizontalArrangement = Arrangement.Center
        ) {
            Text (
                "Kernel channel: ",
                fontSize = 16.sp
            )
            Text (
                "t.me/magictimekernel",
                Modifier
                    .clickable{
                        val intent = Intent(Intent.ACTION_VIEW, "https://t.me/magictimekernel".toUri())
                        context.startActivity(intent)
                    },
                color = MaterialTheme.colorScheme.primary,
                textDecoration = TextDecoration.Underline,
                fontSize = 16.sp,
            )
        }
    }
}

@Preview(showBackground = true)
@Composable
fun GreetingPreview() {
    TIMISONGTheme {
        Greeting()
    }
}
```
