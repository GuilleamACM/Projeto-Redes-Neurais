# Projeto-Redes-Neurais

Projeto final da disciplina de Redes Neurais 2020.2 - CIn UFPE 

# Planejamento do Projeto

Modelos que vamos fazer =
        neural network:             MLP e CNN.
        ensembles:                  Ensemble MLP, Ensemble CNN.
        outros classificadores:     Random Forest, SVM e XGboost.


Primeiro passo, tuning de hyperparametros com neural network de apenas uma camada.

    hyperparametros (entre varios) que poderão ser testados (talvez com auxilio de gridsearch ou semelhante):
        batch-size
        hidden_layer_sizes
        activation
        solver
        alpha
        learning_rate

em geral pretendemos usar este paper como referencia para o tuning: http://yann.lecun.com/exdb/publis/pdf/lecun-98b.pdf

Segundo passo, tuning de hyperparametros das neural networks com multiplas camadas. Em seguida vamos comparar resultados com o primeiro passo e escolher os melhores para formar os emsembles. Como será feita a escolha ainda será debatido, talvez os que possuírem valores de alguma metrica especifica elevada.

Tercerio passo, validação cruzada.

Quarto passo, redução de dimensionalidade + validação cruzada. Caso a redução de dimensionalidade dê resultados positivos, vamos mantê-la. Caso contrario, ignoramos este passo e seguimos para o seguinte.

Quinto passo, formação dos ensembles. O grupo ainda vai tomar uma decisão sobre qual será escolhido. Algumas possibilidades são BaggingClassifier, VotingClassifier e StackingClassifier.
