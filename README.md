![TIMISONG's Git Stats](https://github-readme-stats.vercel.app/api?username=timisong-dev&theme=dark&layout=compact)
![Favorite Lang's](https://github-readme-stats.vercel.app/api/top-langs/?username=timisong-dev&theme=dark&layout=compact)


```kotlin
package timisongdev.timisong

import android.os.Bundle
import android.developer               
import rhythm.guitarist               
import android.designer
import kernel.developer
import developer.java*
import developer.c*
import developer.kotlin*
import developer.flutter*
import developer.kotlin.compose*
import developer.kotlin.multiplatform*
import android.annotation.SuppressLint
import android.content.Intent
import android.os.Bundle
import androidx.activity.ComponentActivity
import androidx.activity.compose.setContent
import androidx.activity.enableEdgeToEdge
import androidx.compose.foundation.clickable
import androidx.compose.foundation.layout.*
import androidx.compose.foundation.layout.Arrangement
import androidx.compose.material3.*
import androidx.compose.runtime.Composable
import androidx.compose.ui.*
import androidx.compose.ui.Modifier
import androidx.compose.ui.platform.LocalContext
import androidx.compose.ui.text.font.FontWeight
import androidx.compose.ui.text.style.TextDecoration
import androidx.compose.ui.tooling.preview.Preview
import androidx.compose.ui.unit.*
import timisongdev.timisong.ui.theme.TIMISONGTheme
import androidx.core.net.toUri

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
