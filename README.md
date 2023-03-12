# Practica n5
 ###Ejercicio 1
numArtefactos <- c(17, 54, 10, 34, 90, 33, 49, 82, 12, 23, 56, 78, 44, 102, 10, 53, 4, 28, 37, 95)
###Ejercicio 2
mean(c(17, 54, 10, 34, 90, 33, 49, 82, 12, 23, 56, 78, 44, 102, 10, 53, 4, 28, 37, 95))
###Ejercicio 3
median(c(17, 54, 10, 34, 90, 33, 49, 82, 12, 23, 56, 78, 44, 102, 10, 53, 4, 28, 37, 95))
###Ejercicio 4
calculate_mode <- function(x) {
  ux <- unique(x)
  ux[which.max(tabulate(match(x, ux)))]
calculate_mode(c(17, 54, 10, 34, 90, 33, 49, 82, 12, 23, 56, 78, 44, 102, 10, 53, 4, 28, 37, 95))
###Ejercicio 5
tabla <- table(c(17, 54, 10, 34, 90, 33, 49, 82, 12, 23, 56, 78, 44, 102, 10, 53, 4, 28, 37, 95))
max_ocurrencias <- max(tabla)
valores_moda <- as.numeric(names(tabla[tabla == max_ocurrencias]))
ocurrencias_moda <- max_ocurrencias
###Ejercicio 6
numeros <- c(17, 54, 10, 34, 90, 33, 49, 82, 12, 23, 56, 78, 44, 102, 10, 53, 4, 28, 37, 95)
`quantile´(17, 54, 10, 34, 90, 33, 49, 82, 12, 23, 56, 78, 44, 102, 10, 53, 4, 28, 37, 95)
###Ejercicio 7
IQR(17, 54, 10, 34, 90, 33, 49, 82, 12, 23, 56, 78, 44, 102, 10, 53, 4, 28, 37, 95)
###Ejercicio 8
rango <- diff(range(numeros))
###Ejercicio 9
var(17, 54, 10, 34, 90, 33, 49, 82, 12, 23, 56, 78, 44, 102, 10, 53, 4, 28, 37, 95)
###Ejercicio 10
Sd(numArtefactos_int)
Sqrt(var(numArtefactos_int))
###Ejercicio 12
barplot(datos, horiz = TRUE, main = "Gráfico de barras horizontales")
###Ejercicio 13
vector3 <- c(21, 45, 33, 98, 34, 90, 67, 87, 45, 11, 73, 38, 28, 15, 50, 57, 12, 87, 29, 1)
###Ejercicio 14
datos1 <- c(17, 54, 10, 34, 90, 33, 49, 82, 12, 23, 56, 78, 44, 102, 10, 53, 4, 28, 37, 95)
cv(datos1)
datos2 <- c(21, 45, 33, 98, 34, 90, 67, 87, 45, 11, 73, 38, 28, 15, 50, 57, 12, 87, 29, 1)
cv(datos2)
###Ejercicio 15
stats <- data.frame(Media = mean(numArtefactos_int),
                    Mediana = median(numArtefactos_int),
                    Desv_Estandar = sd(numArtefactos_int),
                    Minimo = min(numArtefactos_int),
                    Maximo = max(numArtefactos_int)
###Ejercicio 16
vector3 <- c(21, 45, 33, 98, 34, 90, 67, 87, 45, 11, 73, 38, 28, 15, 50, 57, 12, 87, 29, 1)
install.packages("e1071") library(e1071)
skewness(vector3)
###Ejercicio17
vector3 = (21, 45, 33, 98, 34, 90, 67, 87, 45, 11, 73, 38, 28, 15, 50, 57, 12, 87, 29, 1)
mean = np.mean(vector3)
std = np.std(vector3, ddof=1)
kurt = np.sum((vector3 - mean)**4)/len(vector3) / std**4 - 3
print("La curtosis del vector es:", kurt)
