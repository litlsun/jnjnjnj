```mermaid
graph TD
    %% Root Node
    AphasiaOntology[Aphasia Ontology]

    %% Main Classes
    AphasiaOntology --> AphasiaForm
    AphasiaOntology --> SpeechMarker

    %% AphasiaForm Branch
    AphasiaForm --> MotorAphasia
    AphasiaForm --> SensoryAphasia

    MotorAphasia --> EfferentMotorAphasia
    MotorAphasia --> AfferentMotorAphasia
    MotorAphasia --> DynamicAphasia

    SensoryAphasia --> AcousticAgnosticAphasia
    SensoryAphasia --> AcousticMnemonicAphasia

    %% SpeechMarker Branch
    SpeechMarker --> Paraphasia
    SpeechMarker --> StructuralDisorder
    SpeechMarker --> SpeechDynamicsDisorder

    Paraphasia --> LiteralParaphasia
    Paraphasia --> VerbalParaphasia

    StructuralDisorder --> Agrammatism
    StructuralDisorder --> Neologism

    SpeechDynamicsDisorder --> Embolia
    SpeechDynamicsDisorder --> Logorrhea
