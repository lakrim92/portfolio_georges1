---
title: "Exemples de Shortcodes"
date: 2020-06-08T08:06:25+06:00
description: Exemple de shortcodes
menu:
  sidebar:
    name: Exemple de Shortcodes
    identifier: shortcodes
    weight: 40
hero: boat.jpg
mermaid: true
---

Ceci est un article exemple destiné à tester les éléments suivants :

- Image de héros par défaut.
- Différents shortcodes.

## Alerte

Les alertes suivantes sont disponibles dans ce thème.

{{< alert type="success" >}}
Ceci est une alerte exemple avec `type="success"`.
{{< /alert >}}

{{< alert type="danger" >}}
Ceci est une alerte exemple avec `type="danger"`.
{{< /alert >}}

{{< alert type="warning" >}}
Ceci est une alerte exemple avec `type="warning"`.
{{< /alert >}}

{{< alert type="info" >}}
Ceci est une alerte exemple avec `type="info"`.
{{< /alert >}}

{{< alert type="dark" >}}
Ceci est une alerte exemple avec `type="dark"`.
{{< /alert >}}

{{< alert type="primary" >}}
Ceci est une alerte exemple avec `type="primary"`.
{{< /alert >}}

{{< alert type="secondary" >}}
Ceci est une alerte exemple avec `type="secondary"`.
{{< /alert >}}

## Image

#### Une image exemple sans aucun attribut.

{{< img src="/posts/shortcodes/boat.jpg" title="Un bateau en mer" >}}

{{< vs 3 >}}

#### Une image exemple avec les attributs `height` et `width`.

{{< img src="/posts/shortcodes/boat.jpg" height="400" width="600" title="Un bateau en mer" >}}

{{< vs 3 >}}

#### Une image centrée avec les attributs `height` et `width`.

{{< img src="/posts/shortcodes/boat.jpg" height="400" width="600" align="center" title="Un bateau en mer" >}}

{{< vs 3 >}}

#### Une image avec l'attribut `float`.

{{< img src="/posts/shortcodes/boat.jpg" height="200" width="500" float="right" title="Un bateau en mer" >}}

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras egestas lectus sed leo ultricies ultricies. Praesent tellus risus, eleifend vel efficitur ac, venenatis sit amet sem. Ut ut egestas erat. Fusce ut leo turpis. Morbi consectetur sed lacus vitae vehicula. Cras gravida turpis id eleifend volutpat. Suspendisse nec ipsum eu erat finibus dictum. Morbi volutpat nulla purus, vel maximus ex molestie id. Nullam posuere est urna, at bningilla eros venenatis quis.

Fusce vulputate dolor augue, ut porta sapien bningilla nec. Vivamus commodo erat felis, a sodales lectus finibus nec. In a pulvinar orci. Maecenas suscipit eget lorem non pretium. Nulla aliquam a augue nec blandit. Curabitur ac urna iaculis, ornare ligula nec, placerat nulla. Maecenas aliquam nisi vitae tempus vulputate.

## Séparation

Ce thème prend en charge la division de la page en autant de colonnes que vous le souhaitez.

#### Division en deux colonnes

{{< split 6 6 >}}

##### Colonne de gauche

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras egestas lectus sed leo ultricies ultricies.

---

##### Colonne de droite

Fusce ut leo turpis. Morbi consectetur sed lacus vitae vehicula. Cras gravida turpis id eleifend volutpat.

{{< /split >}}

#### Division en trois colonnes

{{< split 4 4 4 >}}

##### Colonne de gauche

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras egestas lectus sed leo ultricies ultricies.

---

##### Colonne du milieu

Aenean dignissim dictum ex. Donec a nunc vel nibh placerat interdum. 

---

##### Colonne de droite

Fusce ut leo turpis. Morbi consectetur sed lacus vitae vehicula. Cras gravida turpis id eleifend volutpat.

{{< /split >}}

## Espace Vertical

Ajoutez un espace vertical entre deux lignes.

Ceci est la première ligne.
{{< vs 4 >}}
Ceci est la deuxième ligne. Elle devrait avoir un espace vertical de `4rem` avec la ligne précédente.

## Vidéo

{{< video src="/videos/sample.mp4" >}}

<!-- markdown-link-check-disable-next-line -->
Vidéo de [Rahul Sharma](https://www.pexels.com/@rahul-sharma-493988) provenant de [Pexels](https://www.pexels.com).

## Mermaid

Voici quelques exemples de shortcode mermaid.

**Graphique:**

{{< mermaid align="left" >}}
graph LR;
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
{{< /mermaid >}}

**Diagramme de séquence:**

{{< mermaid >}}
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>Georges: Bonjour Georges, comment ça va?
    loop Vérification de la santé
        Georges->>Georges: Lutte contre l'hypocondrie
    end
    Note right of Georges: Les pensées rationnelles <br/>préviennent!
    Georges-->>Alice: Super!
    Georges->>Bob: Et toi?
    Bob-->>Georges: Très bien!
{{< /mermaid >}}

**Diagramme de Gantt:**

{{< mermaid >}}
gantt
  dateFormat  YYYY-MM-DD
  title Ajout du diagramme de GANTT à mermaid
  excludes weekdays 2014-01-10

section Une section
  Tâche terminée            :done,    des1, 2014-01-06,2014-01-08
  Tâche active               :active,  des2, 2014-01-09, 3d
  Tâche future               :         des3, after des2, 5d
  Tâche future2              :         des4, after des3, 5d
{{< /mermaid >}}

**Diagramme de classe:**

{{< mermaid >}}
classDiagram
  Class01 <|-- AveryLongClass : Cool
  Class03 *-- Class04
  Class05 o-- Class06
  Class07 .. Class08
  Class09 --> C2 : Où suis-je?
  Class09 --* C3
  Class09 --|> Class07
  Class07 : equals()
  Class07 : Object[] elementData
  Class01 : size()
  Class01 : int chimp
  Class01 : int gorilla
  Class08 <--> C2: Étiquette cool
{{< /mermaid >}}

**Graphique Git:**

{{< mermaid >}}
gitGraph
    commit id: "ZERO"
    branch develop
    commit id:"A"
    checkout main
    commit id:"ONE"
    checkout develop
    commit id:"B"
    checkout main
    commit id:"TWO"
    cherry-pick id:"A"
    commit id:"THREE"
    checkout develop
    commit id:"C"
{{< /mermaid >}}

**Diagramme ER:**

{{< mermaid >}}
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
{{< /mermaid >}}

## Gist

{{< gist hossainemruz 4ad86c9b6378677e14eff12713e75e44 >}}

## PDF Intégré

{{< embed-pdf src="/files/resume.pdf" >}}
