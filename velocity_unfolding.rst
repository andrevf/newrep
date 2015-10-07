Velocity Unfolding
=================

Há limitações na medição da velocidade radial que dependem da frequencia utilizada pelo radar. Um radar que utilize a frequencia xHz, por exemplo, consegue medir velocidades entre -10m/s e 10m/s. Para velocidades fora deste intervalo ocorre um "dobramento": se a velocidade real é de 15m/s, por exemplo, a velocidade medida será -5m/s. Para contornar esta limitação pode-se coletar os dados de maneira diferente, alterarando o funcionamento do radar, ou pode-se tratar os dados depois de coletados.

Depois de coletados os dados, existem técnicas para fazer as devidas correções. O *pyart* tem duas delas implementadas:

* pyart.correct.dealias_region_based();
* pyart.correct.dealias_unwrap_phase().

