


<nb-select placeholder="Sélectionnez une option" [(ngModel)]="selectedOption">
  <nb-option *ngFor="let option of options" [value]="option.value">{{ option.label }}</nb-option>
</nb-select>

<!-- Formulaire pour l'option 1 -->
<div *ngIf="selectedOption === 'option1'">
  <h2>Formulaire pour l'option 1</h2>
  <!-- Ajoutez les champs de formulaire nécessaires ici -->
</div>

<!-- Formulaire pour l'option 2 -->
<div *ngIf="selectedOption === 'option2'">
  <h2>Formulaire pour l'option 2</h2>
  <!-- Ajoutez les champs de formulaire nécessaires ici -->
</div>


  options = [
    { value: 'option1', label: 'Option 1' },
    { value: 'option2', label: 'Option 2' }
  ];


  selectedOption: string | undefined;
