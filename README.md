import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Github, Linkedin, Mail } from "lucide-react";
import { motion } from "framer-motion";

export default function Portfolio() {
  return (
    <div className="min-h-screen bg-gray-900 text-white p-6">
      {/* Header */}
      <header className="text-center py-8">
        <h1 className="text-4xl font-bold">👋 Hi, I'm Prince Pal</h1>
        <p className="mt-2 text-lg text-gray-300">
          🎓 B.Tech CSE (Data Science) | DIT University, Dehradun
        </p>
        <p className="text-gray-400">
          💡 Data Science | Machine Learning | AI | Software Development
        </p>
      </header>

      {/* About Me */}
      <motion.section
        className="max-w-3xl mx-auto mb-12"
        initial={{ opacity: 0, y: 40 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 0.8 }}
      >
        <Card className="bg-gray-800 border-none shadow-xl">
          <CardContent className="p-6 space-y-4">
            <h2 className="text-2xl font-semibold">🧑‍💻 About Me</h2>
            <ul className="list-disc pl-5 text-gray-300 space-y-2">
              <li>Currently pursuing B.Tech in CSE (Data Science)</li>
              <li>Interested in Machine Learning, Data Analytics, and Deep Learning</li>
              <li>Building projects with Python, SQL, and AI frameworks</li>
              <li>Open to collaborating on Data Science & Open Source Projects</li>
              <li>Goal: Create impactful data-driven solutions</li>
            </ul>
          </CardContent>
        </Card>
      </motion.section>

      {/* Tech Stack */}
      <motion.section
        className="max-w-4xl mx-auto mb-12"
        initial={{ opacity: 0, y: 40 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 1 }}
      >
        <Card className="bg-gray-800 border-none shadow-xl">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-4">🛠️ Tech Stack</h2>
            <div className="grid grid-cols-2 sm:grid-cols-3 gap-4 text-gray-300">
              <p>Python</p>
              <p>C++</p>
              <p>SQL</p>
              <p>R</p>
              <p>Pandas</p>
              <p>NumPy</p>
              <p>Matplotlib</p>
              <p>Scikit-Learn</p>
              <p>MySQL</p>
              <p>MongoDB</p>
              <p>Git/GitHub</p>
              <p>Data Visualization</p>
            </div>
          </CardContent>
        </Card>
      </motion.section>

      {/* GitHub Stats - Embed */}
      <motion.section
        className="text-center mb-12"
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        transition={{ duration: 1.2 }}
      >
        <h2 className="text-2xl font-semibold mb-4">📊 GitHub Stats</h2>
        <div className="flex flex-col sm:flex-row items-center justify-center gap-4">
          <img
            src="https://github-readme-stats.vercel.app/api?username=PrincePal&show_icons=true&theme=tokyonight"
            alt="GitHub Stats"
            className="rounded-xl shadow-lg"
          />
          <img
            src="https://github-readme-stats.vercel.app/api/top-langs/?username=PrincePal&layout=compact&theme=tokyonight"
            alt="Top Languages"
            className="rounded-xl shadow-lg"
          />
        </div>
      </motion.section>

      {/* Contact */}
      <motion.section
        className="text-center"
        initial={{ opacity: 0, y: 40 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 1.4 }}
      >
        <h2 className="text-2xl font-semibold mb-4">🌐 Connect with Me</h2>
        <div className="flex justify-center gap-4">
          <Button
            variant="outline"
            className="bg-gray-800 text-white border-gray-700 hover:bg-gray-700"
            asChild
          >
            <a href="https://github.com/PrincePal" target="_blank">
              <Github className="mr-2 h-4 w-4" /> GitHub
            </a>
          </Button>
          <Button
            variant="outline"
            className="bg-gray-800 text-white border-gray-700 hover:bg-gray-700"
            asChild
          >
            <a href="https://www.linkedin.com/" target="_blank">
              <Linkedin className="mr-2 h-4 w-4" /> LinkedIn
            </a>
          </Button>
          <Button
            variant="outline"
            className="bg-gray-800 text-white border-gray-700 hover:bg-gray-700"
            asChild
          >
            <a href="mailto:your-email@example.com">
              <Mail className="mr-2 h-4 w-4" /> Email
            </a>
          </Button>
        </div>
      </motion.section>

      {/* Footer */}
      <footer className="text-center mt-12 text-gray-500">
        ⭐️ “Turning data into meaningful insights to build a smarter future.”
      </footer>
    </div>
  );
}
