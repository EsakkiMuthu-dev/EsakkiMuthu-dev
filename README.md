# 👋 Welcome to My GitHub Profile

```rust
println!("👋 Hello there! Let’s meet Esakki Muthu!");

struct EsakkiMuthu {
    username: &'static str,
    name: &'static str,
    position: &'static str,
    blog: &'static str,
    socials: Socials,
    code: Code,
    architecture: [&'static str; 4],
}

struct Socials {
    twitter: &'static str,
    github: &'static str,
    linkedin: &'static str,
}

struct Code {
    backend: [&'static str; 5],
    database: [&'static str; 4],
    devops: [&'static str; 3],
    frontend: [&'static str; 5],
    tools: [&'static str; 4],
}

fn main() {
    let me = EsakkiMuthu {
        username: "esakkimuthu",
        name: "Esakki Muthu",
        position: "Backend Developer at Zoho",
        blog: "https://esakkimuthu-portfolio.vercel.app/",
        socials: Socials {
            github: "https://github.com/EsakkiMuthu-dev",
            linkedin: "https://www.linkedin.com/in/esakkimuthu-esakki/",
        },
        code: Code {
            backend: ["Java", "Node.js", "Python", "Rust", "Spring Boot"],
            database: ["PostgreSQL", "MySQL", "MongoDB", "SQLite"],
            devops: ["Linux", "Google Cloud", "Github Actions"],
            frontend: ["React", "HTML", "CSS", "JavaScript", ],
            tools: ["Postman","VSCode", "GitHub", "Docker", "IntelliJ","Firebase"],
        },
        architecture: ["MVC", "Microservices", "Serverless", "SPA"],
    };

    println!(
        "{} is a {} who codes in {} and builds {}!",
        me.name,
        me.position,
        me.code.backend.join(", "),
        me.architecture.join(" and ")
    );
}
