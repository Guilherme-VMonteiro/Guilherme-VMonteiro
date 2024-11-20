```
@Entity
@Table(name = "about_me") 
public class AboutMe {

  private String name = "Guilherme Monteiro"

  @ColumnDefault("Full Stack")
  private String area = "QA"

  private List<String> skills = Arrays.asList("Angular", "Spring", "Cypress", "WebDriverIO");
}
```

<p align="center">
<img src="https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExZ2s2Z3VycHhxaGMxam9jdmd4NGdodHp6cnVyaHByaDJzZnA4ZTBleSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/22CEvbj04nLLq/giphy.gif">
</p>
