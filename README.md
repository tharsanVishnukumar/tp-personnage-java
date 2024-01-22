# Personnagev1

Projet Personnage initial

Premier projet objet

package Personnage;

public class Personnage {
private String nom;
private int vie;

    public Personnage(String nom, int vie) {
        this.nom = nom;
        this.vie = vie;
    }

    public String LeNom() {
        return this.nom;
    }

    public int LaVie() {
        return this.vie;
    }

    public void AugmenterVie(int vie) {
        this.vie += vie;
    }

    public void Attaque(Personnage perso, int domage) {
        perso.vie -= domage / 2;
        this.vie -= domage / 2;
    }

}
