---
title: 'Configuration requise pour la déclaration d’échanges de biens [FR]'
description: Cet article présente une liste des champs requis pour la déclaration d’échanges de biens (DEB) au format DTI+ dans la version française de Business Central.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 05/09/2022
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# <a name="requirements-for-reporting-declaration-of-trade-in-goods-in-the-french-version"></a>Configuration requise pour la déclaration d’échanges de biens dans la version française

Dans cet article, nous décrivons comment configurer votre [!INCLUDE [prod_short](../../includes/prod_short.md)] pour la déclaration d’échanges de biens (DEB) en France.  

Les champs suivants sont requis pour la déclaration d’échanges de biens :  

- **CISD** dans la table **Informations société**.  
- **N° SIRET** dans la table **Informations société**.  
- **N° identif. intracomm.** dans la table **Informations société**.  
- **Nom** dans la table **Informations société**.  
- **Date** de la période statistique dans la table **Ligne feuille intracomm**.  
- **Régime** dans la table **Ligne feuille intracomm**.  
- La **Quantité** dans la table **Ligne feuille intracomm** doit être supérieure à 0.  
- La **Valeur statistique** dans la table **Ligne feuille intracomm** doit être supérieure à 0.  

> [!NOTE]  
> L’état **Exporter DEB DTI** exporte les expéditions et les réceptions dans un lot. Si vous souhaitez déclarer uniquement les expéditions ou les réceptions, vous devez définir un filtre pour supprimer les lignes qui ne sont pas nécessaires dans la table **Feuille intracomm**.  

## <a name="intrastat-requirements-for-deb"></a>Configuration requise en matière d’état communautaire pour DEB

Pour la France, la gestion des états communautaires implique de séparer les données déclaratives pour le reporting statistique et pour le reporting fiscal (état récapitulatif de la TVA). Il est nécessaire que l’état communautaire exporte les fichiers séparément en fonction du niveau d’obligation configuré.

1. Pour exporter les lignes de l’état communautaire correctement, sélectionnez l’icône ![Ampoule qui ouvre la fonction de recherche.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , saisissez **Feuilles intracommunautaires**, puis sélectionnez l’action **Suggérer des lignes**. De nouvelles lignes feuille communautaire sont créées pour la période sélectionnée.  

2. Dans les lignes feuille, renseignez les champs nécessaires, puis sélectionnez l’action **Exporter DEB DTI+**.  

    L’action **Exporter DEB DTI** est exécutée. Vous devez préciser le niveau d’obligation à déclarer. Le champ **Filtre régime** sur la page de la demande a une valeur prédéfinie qui dépend du niveau d’obligation précisé. La valeur de ce champ est un filtre qui s’applique au champ **Régime** des lignes feuille intracommunautaire.  

Lorsque l’état est exécuté, seules les lignes feuille intracommunautaire dont la valeur du champ **Régime** correspond au champ **Filtre régime** sont traitées. Le champ **Filtre régime** est modifiable, vous pouvez donc modifier sa valeur en fonction de vos besoins. Le tableau suivant décrit les valeurs actuellement prises en charge :

| Niveau | Filtrer |
|--|--|
| **Niveau d’obligation 1** | `11 | 19 | 21 | 29` |
| **Niveau d’obligation 2** | "" (filtre vide pour que toutes les lignes feuille intracommunautaire soient traitées) |
| **Niveau d’obligation 3** | "" |
| **Niveau d’obligation 4** | `<>29&<>11&<>19` (les lignes avec le régime 29, 11, 19 ne sont pas traitées) |
| **Niveau d’obligation 5** | `<>11&<>19` |

## <a name="validate-intrastat-lines"></a>Valider les lignes intracommunautaires

Exécutez l’état **Liste de contrôle de la déclaration d’échanges de biens avancée** pour vérifier les lignes feuille intracommunautaire avant leur exportation au format XML. La vérification est exécutée dans l’état **Exporter DEB DTI**.  

### <a name="to-enable-the-check"></a>Pour activer la vérification

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction de recherche.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") , saisissez **Configuration intracomm.**, puis choisissez le lien approprié.  
2. Sélectionnez le champ **Utiliser la liste de contrôle avancée**.  
3. Sélectionnez l’action **Paramètres liste de contrôle de la déclaration d’échanges de biens avancée**.
4. Ajoutez les lignes nécessaires en définissant le champ **Type d’objet** sur *État* et le champ **ID objet** sur *10821*. Puis définissez le champ **N° champ** sur un champ qui doit être vérifié pour une valeur non vide. Remplissez le champ **Expression de filtre** si nécessaire.

## <a name="see-also"></a>Voir aussi

[Fonctionnalité locale, France](france-local-functionality.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
