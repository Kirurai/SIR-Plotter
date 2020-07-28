# SIR-Plotter  
  
Contribuyentes
--
[De Filippi Bruno](https://github.com/bdefilippi)  
[Henriquez Agustín](https://github.com/AgustinHenriquez)  
[Miño Maurizio](https://github.com/MaurizioMi)  
  
Tema Propuesto:
--
Simulador de brote/contagios de pandemia.  
  
Características principales:
--
+ Mostrar un gráfico estadístico durante el tiempo.  
+ Contar con un filtro para modificar variables y así poder generar nuevos casos de estudio.  
+ Permitir el guardado de simulaciones anteriores para poder realizar comparaciones.  
  
El programa utilizaría una serie de cálculos matemáticos y variables para simular cada una de las situaciones de contagio,  
entre las cuales podríamos contar con variables como:  
+ Tamaño de la muestra  
+ Rango de infección del virus  
+ Tiempo de recuperación del virus, taza de mortalidad  
+ Variables especiales como lo serían el distanciamiento social y la cuarentena  
  
El programa se basa en un modelo SIR, lo que significa que la población se reparte en tres categorías:  
+ Susceptibles: Aquellos que son susceptibles a contraer una enfermedad (S)  
+ Infecciosos: Aquellos que se encuentran actualmente contagiados (I)  
+ Recuperados o Removidos: Aquellos que se han recuperado o han fallecido por la enfermedad, por lo tanto no son considerados  
un factor nuevo de contagio. (R)  
  
Manual de uso
--
  
1) Ejecutar LAUNCHER.sh  
  
2) En la ventana de Edición de parametros, tenemos varias opciones:  
  
*Probabilidad de Remoción: Es la chance que tiene una persona Infectada de ser Removida.  
*Probabilidad de Infección: Es la chance que tiene una persona Susceptible de ser contagiada por una persona Infectada.  
  **Valor Incial: Determina el valor al inicio del experimento para la variable.  
  **Valor Final: Determina el valor de la variable luego de transcurridos los "Dias de Cambio", dejarlo con el mismo valor a Valor Inicial en caso de no querer que se produzcan cambios en el tiempo.  
  **Dias de Cambio: Numero de dias para que se produzca un cambio en los valores de las variables.  
  
*Población Incial, Susceptibles: Personas Susceptibles a contagio en la población.  
*Pobalcion Inicial, Infectados: Personas Infectadas en la población.  
  
3) Presionar el botón "Cargar parámetros" para ejecutar la simulación con los parámetros actuales. Aparecerá una alerta cuando la simulación haya concluído.  
  
4) Presionar el botón "Graficar!" para obtener una representación gráfica del último experimento realizado.  
  
5) Presionar el botón "Valores por defecto" para reiniciar los valores por defecto.  
  
6) Presionar el botón "Más detalles" para poder ver el .csv con los datos del último experizmento. (requiere un lector de .csv instalado en el equipo). En el mismo hay 4 columnas, las cuales representan:  
  1. tiempo: El tiempo en el que se ha realizado cada prueba (en días)  
  2. S: Personas Susceptibles.  
  3. I: Personas Infectadas.  
  4. R: Personas Removidas.  
    
7) Presionar el botón "Histórico" para poder ver el .csv con los datos de todos los experimentos realizados. (requiere un lector de .csv instalado en el equipo). En el mismo hay 14 columnas, las cuales representan:  
  1. fecha_del_experimento: La fecha del experimento, incluye la hora a la que se realizó el mismo.  
  2. mu_inicial: Valor inicial de mu. (Probabilidad de Remoción)  
  3. mu_final: Valor final de mu. (Probabilidad de Remoción)  
  4. mu_dias_cambio: Numero de dias para que se produzca un cambio en mu.  
  5. beta_inicial: Valor inicial de beta. (Probabilidad de Infección)  
  6. beta_final:	Valor final de beta. (Probabilidad de Infección)  
  7. beta_dias_cambio: Numero de dias para que se produzca un cambio en beta.  
  8. S0: Valor incial de Susceptibles  
  9. I0: Valor incial de Infectados  
  10. R0: Valor incial de Removidos  
  11. tiempo: El tiempo total (en días) de duración del experimento.    
  12. S: Valor final de Susceptibles  
  13. I: Valor final de Susceptibles  
  14. R: Valor final de Susceptibles  
    
Necesario para correr el programa
--
Tener instalado Python 3.6 y pip3 por lo menos. En Linux deben estar en los comandos de python y pip respectivamente en lugar de python2.7 se puede confirmar con python --version en la consola  
instalar miniconda de https://conda.io/projects/conda/en/latest/user-guide/install/linux.html  
instalar mediante el comando conda matplotlib, numpy y pandas  

Utilizados:
--
Lenguaje usado: Python 3.7  
Ide utilizado: Pycharm  
Estado actual: Finalizado  
