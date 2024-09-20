# Model Predykcyjny dla Prognozowania Temperatury i Ciśnienia Atmosferycznego

Projekt ten koncentruje się na opracowaniu modelu predykcyjnego do prognozowania temperatury i ciśnienia atmosferycznego w oparciu o dane czasowe. Wykorzystuje sieć rekurencyjną LSTM (Long Short-Term Memory), która jest szczególnie skuteczna w analizie sekwencji danych, takich jak zmienne meteorologiczne.

Dane pochodzą ze strony https://www.kaggle.com/datasets/budincsevity/szeged-weather. Dotyczą one pogody w mieście Segedyn na Węgrzech. Dane zawierają godzinowe pomiary w latach 2006-2016. Dane zawierają zmienne takie jak:
- Formatted Date;
- Precip Type;
- Temperature (C);     
- Apparent Temperature (C); 
- Humidity;
- Wind Speed (km/h);    
- Wind Bearing (degrees);    
- Visibility (km);           
- Pressure (millibars);      
- Daily Summary.

## Model końcowy

Najlepszy model osiągnął wynik <b>MSE</b> dla:
- Temperature: 1.08;
- Pressure: 1.04.

Konstrukcja modelu:
<p align="center">
  <img src="/plots/model.png">
</p>

### Wyniki na zbiorze testowym

Wykres wartości przewidywanych względem rzeczywistych dla temperatury
<p align="center">
  <img src="/plots/pred_temp.png">
</p>

Wykres wartości przewidywanych względem rzeczywistych dla ciśnienia
<p align="center">
  <img src="/plots/pred_press.png">
</p>

## Porównanie z innymi stworzonymi modelami
<p align="center">
  <img src="/plots/summ_table.png">
</p>

## Materiały pomocnicze

https://blog.davidkaleko.com/feature-engineering-cyclical-features.html
