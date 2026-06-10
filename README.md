# projekt-programowanie
dane pochodzą z https://archive.ics.uci.edu/dataset/373/drug+consumption+quantified

zbiór zawiera 1885 wierszy (osób, które wypełniły ankietę) i 32 kolumny 

w ankiecie pobrano dane o cechach osobowości i używania substancji psychoaktywnych

wyróżniono następujące cechy: Age - Wiek respondenta, Gender - Płeć, Education - Poziom wykształcenia, Country - Kraj zamieszkania, Nscore - Neurotyczność (Big Five), Escore - Ekstrawersja (Big Five), Oscore - Otwartość na doświadczenia (Big Five), Ascore - Ugodowość (Big Five), Cscore - Sumienność (Big Five), Impulsive - Impulsywność, SS - Poszukiwanie wrażeń

celem projektu jest przewidywanie czy dana osoba brała LSD na podstawie jej cech osobowości i demograficznych

w projekcie zostały użyte dwa modele klasyfikacji: regresja logistyczna i random forest

kolumnę LSD uproszczono, z 6 kategorii do 2, 0 = nie brał, 1 = brał

dodatkowo usuwamy wiersze osób, które zaznaczyły że brały fikcyjny narkotyk semeron

wyniki - 
regresja logistyczna: accuracy: 0.74, f1-score: 0.72
random forest: accuracy: 0.78 f1-score: 0.76

random forest okazał się lepszym modelem a najsilniejszymi cechami były oscore i ss (otwartość i poszukiwanie doświadczeń)
