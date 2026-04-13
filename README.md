# Proyecto-Clima
Intento de IA para predecir eventos climáticos. Datos obtenidos de AEMET
# Si hay alertas, guardamos un archivo especial de incidencias
if not ciudades_en_alerta.empty:
    nombre_alerta = f"ALERTA_CALOR_{fecha_hoy}.csv"
    ciudades_en_alerta.to_csv(nombre_alerta, index=False)
    print(f"📝 Se ha generado un registro de incidencias en: {nombre_alerta}")
