Si los servicios de las {% data variables.product.prodname_actions %} se encuentran temporalmente no disponibles, entonces se descartará una ejecución de flujo de trabajo si no se puso en cola en los primeros 30 minutos después de activarse. Por ejemplo, si un flujo de trabajo se activa y los servicios de las {% data variables.product.prodname_actions %} no están disponibles por 31 minutos o más, entonces la ejecución de flujo de trabajo no se procesará.