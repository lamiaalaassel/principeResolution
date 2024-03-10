# principeResolution
Le code implémente un solveur logique propositionnel basé sur l'algorithme de résolution. Voici un résumé des principales fonctions :

1.parse_formula_input(input_string) : Cette fonction extrait les clauses d'une formule logique au format DNF (forme normale disjonctive) à partir d'une chaîne de caractères en utilisant des expressions régulières. Les clauses sont ensuite converties en listes de littéraux.

2.negation(F) : Cette fonction génère la formule négative d'une formule logique donnée. Chaque littéral dans chaque clause est inversé.

3.mettre_sous_forme_de_clauses(F) : Cette fonction assure que la formule logique est représentée sous forme de listes de clauses.

4.chercher_clauses_resolvantes(clauses) : Cette fonction identifie les paires de clauses ayant des littéraux complémentaires et génère de nouvelles clauses résultantes de la résolution.

5.resolution(F) : Cette fonction applique l'algorithme de résolution sur une formule logique donnée. Elle utilise la négation de la formule d'entrée, recherche continuellement de nouvelles clauses résolvantes, et détermine si la formule est valide ou invalide.

6.test_resolution() : Cette fonction permet à l'utilisateur d'entrer une formule logique. Elle utilise les fonctions précédentes pour traiter la formule et affiche le résultat de la résolution.

L'exécution du programme consiste à appeler test_resolution(), où l'utilisateur peut saisir une formule logique, et le programme affiche si la formule est valide (exemple:  {PvQ}) ou invalide (exemple :{¬P v ¬Q v R, ¬R, P, ¬T v Q, T}) en utilisant la résolution logique propositionnelle.
