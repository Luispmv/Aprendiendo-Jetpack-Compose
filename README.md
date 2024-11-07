
# Practica en Jetpack Compose

Creacion de componentes en Jetpack Compose

## Mi primer Composable
```kotlin
@Composable
    private fun personalData(name:String){
        MaterialTheme() {
            Column() {
                Image(
                    painter = painterResource(R.drawable.messi),
                    contentDescription = "messi",
                    modifier = Modifier.fillMaxWidth(),
                    contentScale = ContentScale.Crop
                )
                
                Spacer(modifier = Modifier.height(16.dp))

                Column(
                    modifier = Modifier.padding(16.dp)
                ) {
                    Text(text = "Mi nombre es ${name}", style = MaterialTheme.typography.headlineMedium)
                    Text(text = "Tengo 35 años")
                    Text(text = "Soy el mejor jugador de todos los tiempos")
                }
            }
        }
    }

    @Preview
    @Composable
    fun previewPersonalData(){
        personalData("Messi")
    }

```

