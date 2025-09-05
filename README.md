struct Me {
    name: &'static str,
    nationality: &'static str,
    interests: Vec<&'static str>,
    current_project: &'static str,
    languages: Vec<&'static str>,
    contacts: Vec<&'static str>,
}

impl Me {
    fn new() -> Self {
        Self {
            name: "nut",
            nationality: "Thai",
            interests: vec!["Linux", "Web Development", "Ai"],
            current_project: "https://github.com/FewLy-Torch-1861/FewLy-Torch-1861.github.io",
            languages: vec!["Python", "Rust", "JavaScript"],
            contacts: vec![
                "Linktree: FuryTorch"
                "Discord: fury.torch",
            ],
        }
    }

    fn about(&self) {
        println!("👋 Hi, I'm {} from {}", self.name, self.nationality);
        println!("🔥 Interests: {:?}", self.interests);
        println!("🚧 Currently working on: {}", self.current_project);
        println!("💻 Mostly coding in: {:?}", self.languages);
        println!("📫 Contact me: {:?}", self.contacts);
    }
}

fn main() {
    let me = Me::new();
    me.about();
}