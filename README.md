# Simple Sales Dashboard


## Consideraciones: 
- Los datos empleados no son datos reales.
-  Fuentes de datos en formato de texto .csv.
-   Las 3 tablas: Productos, Vendedores y Ventas, están en una relación de uno a muchos.

  
      <details>
       <summary>Modelado de datos</summary>
       <img width="1276" height="809" alt="image" src="https://github.com/user-attachments/assets/3a8fefbd-d9c5-4fb6-be44-969c4c1dd04d" />
     </details>
- Medidas empleadas con DAX:
   - <code>Unidades Vendidas = SUM(Ventas[Unidades])</code>
   - <code>Productos Distintos = DISTINCTCOUNT(Ventas[CódigoProducto])</code>
   - <code>Porcentaje de Ventas = DIVIDE([Unidades Vendidas],CALCULATE([Unidades Vendidas],ALL(Vendedores[Representante])))</code>
- Dashboard diseñado para escritorio y entorno mobile:
    <details>
       <summary>Escritorio</summary>
       <img width="1777" height="978" alt="image" src="https://github.com/user-attachments/assets/73e82d59-e64d-4c56-8c8a-3e1232fdb825" />
    </details>
    <details>
       <summary>Mobile</summary>
       <img width="538" height="886" alt="image" src="https://github.com/user-attachments/assets/e60adaf3-ddf0-4acf-af04-f10324ac0c70" />
       <img width="541" height="916" alt="image" src="https://github.com/user-attachments/assets/f585bc48-3841-4113-8d1b-f1e0090fbb82" />
    </details>
- Si tienes Power BI Desktop instalado en tu PC, descarga el proyecto "Ventas.pbix" y ponlo a prueba. Las fuentes de datos e imágenes son extraídas desde la web.

## Objetivo:
- Analizar las unidades vendidas por producto y vendedor, utilizando elementos gráficos.
