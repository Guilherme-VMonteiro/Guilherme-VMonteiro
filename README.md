```
@Entity
@Table(name = "about_me") 
public class AboutMe {

    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    @Column(name = "name", nullable = false)
    private String name = "Guilherme Monteiro";

    @Column(name = "role")
    @ColumnDefault("'Software Architect'")
    private String role = "Software Developer";

    @ElementCollection
    private List<String> skills = Arrays.asList(
        "Spring Boot", "Angular", "Electron", "Docker", "Kotlin",
        "Microservices", "CI/CD", "Cloud Architecture"
    );

    @OneToMany
    private List<Technology> currentlyLearning = Arrays.asList(
        new Technology("Kotlin"), 
        new Technology("Terraform")
    );

    public void dailyRoutine() {
        while (true) {
            code();
            debug();
            optimizeArchitecture();
            learnSomethingNew();
        }
    }
}

```

<p align="center">
<img src="https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExZ2s2Z3VycHhxaGMxam9jdmd4NGdodHp6cnVyaHByaDJzZnA4ZTBleSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/22CEvbj04nLLq/giphy.gif">
</p>
