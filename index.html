import { useState, useEffect, useCallback } from "react";

const COLORS = {
  bg: "#07070f",
  surface: "#0e0e1c",
  surface2: "#161628",
  surface3: "#1e1e35",
  ue5: "#00c8ff",
  mc: "#3dff8f",
  text: "#dde0ff",
  muted: "#5a5a8a",
  border: "#1e1e3a",
  danger: "#ff4466",
};

const fonts = `
@import url('https://fonts.googleapis.com/css2?family=Rajdhani:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500&family=Bebas+Neue&display=swap');
`;

const css = `
* { box-sizing: border-box; margin: 0; padding: 0; }
body { background: ${COLORS.bg}; color: ${COLORS.text}; font-family: 'Rajdhani', sans-serif; }
::-webkit-scrollbar { width: 4px; } ::-webkit-scrollbar-track { background: ${COLORS.surface}; } ::-webkit-scrollbar-thumb { background: ${COLORS.border}; border-radius: 2px; }
.app { display: flex; height: 100vh; overflow: hidden; }
.sidebar { width: 220px; min-width: 220px; background: ${COLORS.surface}; border-right: 1px solid ${COLORS.border}; display: flex; flex-direction: column; padding: 0; }
.sidebar-logo { padding: 24px 20px 16px; border-bottom: 1px solid ${COLORS.border}; }
.logo-text { font-family: 'Bebas Neue', sans-serif; font-size: 28px; letter-spacing: 3px; background: linear-gradient(90deg, ${COLORS.ue5}, ${COLORS.mc}); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
.logo-sub { font-size: 10px; color: ${COLORS.muted}; letter-spacing: 2px; margin-top: 2px; font-family: 'JetBrains Mono', monospace; }
.nav { padding: 12px 0; flex: 1; }
.nav-item { display: flex; align-items: center; gap: 10px; padding: 10px 20px; cursor: pointer; font-size: 14px; font-weight: 600; letter-spacing: 1px; color: ${COLORS.muted}; transition: all 0.15s; border-left: 2px solid transparent; }
.nav-item:hover { color: ${COLORS.text}; background: ${COLORS.surface2}; }
.nav-item.active { color: ${COLORS.text}; background: ${COLORS.surface2}; border-left-color: ${COLORS.ue5}; }
.nav-item .icon { font-size: 16px; width: 20px; text-align: center; }
.sidebar-footer { padding: 16px 20px; border-top: 1px solid ${COLORS.border}; }
.version { font-family: 'JetBrains Mono', monospace; font-size: 10px; color: ${COLORS.muted}; }
.main { flex: 1; overflow-y: auto; padding: 32px; background: ${COLORS.bg}; }
.page-header { margin-bottom: 28px; }
.page-title { font-family: 'Bebas Neue', sans-serif; font-size: 36px; letter-spacing: 3px; line-height: 1; }
.page-sub { color: ${COLORS.muted}; font-size: 13px; margin-top: 4px; font-family: 'JetBrains Mono', monospace; }
.grid2 { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
.grid3 { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 16px; }
.card { background: ${COLORS.surface}; border: 1px solid ${COLORS.border}; border-radius: 8px; padding: 20px; }
.card-title { font-size: 11px; letter-spacing: 2px; font-weight: 700; color: ${COLORS.muted}; margin-bottom: 8px; }
.card-value { font-family: 'Bebas Neue', sans-serif; font-size: 42px; letter-spacing: 2px; line-height: 1; }
.ue5-color { color: ${COLORS.ue5}; }
.mc-color { color: ${COLORS.mc}; }
.badge { display: inline-flex; align-items: center; padding: 2px 8px; border-radius: 3px; font-size: 11px; font-weight: 700; letter-spacing: 1px; }
.badge-ue5 { background: rgba(0,200,255,0.12); color: ${COLORS.ue5}; border: 1px solid rgba(0,200,255,0.25); }
.badge-mc { background: rgba(61,255,143,0.12); color: ${COLORS.mc}; border: 1px solid rgba(61,255,143,0.25); }
.badge-active { background: rgba(61,255,143,0.12); color: ${COLORS.mc}; border: 1px solid rgba(61,255,143,0.25); }
.badge-paused { background: rgba(90,90,138,0.2); color: ${COLORS.muted}; border: 1px solid ${COLORS.border}; }
.badge-done { background: rgba(0,200,255,0.12); color: ${COLORS.ue5}; border: 1px solid rgba(0,200,255,0.25); }
.btn { display: inline-flex; align-items: center; gap: 6px; padding: 8px 16px; border-radius: 4px; font-family: 'Rajdhani', sans-serif; font-size: 13px; font-weight: 700; letter-spacing: 1px; cursor: pointer; border: none; transition: all 0.15s; }
.btn-primary { background: ${COLORS.ue5}; color: ${COLORS.bg}; }
.btn-primary:hover { background: #33d4ff; }
.btn-mc { background: ${COLORS.mc}; color: ${COLORS.bg}; }
.btn-mc:hover { background: #66ffaa; }
.btn-ghost { background: transparent; color: ${COLORS.muted}; border: 1px solid ${COLORS.border}; }
.btn-ghost:hover { color: ${COLORS.text}; border-color: ${COLORS.muted}; }
.btn-danger { background: transparent; color: ${COLORS.danger}; border: 1px solid rgba(255,68,102,0.3); }
.btn-danger:hover { background: rgba(255,68,102,0.1); }
.btn-sm { padding: 4px 10px; font-size: 11px; }
.input { width: 100%; background: ${COLORS.surface2}; border: 1px solid ${COLORS.border}; border-radius: 4px; padding: 10px 12px; color: ${COLORS.text}; font-family: 'Rajdhani', sans-serif; font-size: 14px; font-weight: 500; outline: none; transition: border 0.15s; }
.input:focus { border-color: ${COLORS.ue5}; }
.textarea { resize: vertical; min-height: 80px; }
.select { appearance: none; cursor: pointer; }
.label { font-size: 11px; font-weight: 700; letter-spacing: 1.5px; color: ${COLORS.muted}; margin-bottom: 6px; display: block; }
.form-group { margin-bottom: 16px; }
.divider { height: 1px; background: ${COLORS.border}; margin: 20px 0; }
.project-card { background: ${COLORS.surface}; border: 1px solid ${COLORS.border}; border-radius: 8px; padding: 18px; cursor: pointer; transition: all 0.15s; position: relative; overflow: hidden; }
.project-card::before { content: ''; position: absolute; top: 0; left: 0; right: 0; height: 2px; }
.project-card.ue5::before { background: ${COLORS.ue5}; }
.project-card.mc::before { background: ${COLORS.mc}; }
.project-card:hover { border-color: ${COLORS.muted}; transform: translateY(-1px); }
.project-name { font-size: 18px; font-weight: 700; letter-spacing: 1px; margin: 8px 0 4px; }
.project-desc { font-size: 13px; color: ${COLORS.muted}; line-height: 1.5; }
.project-meta { display: flex; gap: 8px; align-items: center; margin-top: 12px; flex-wrap: wrap; }
.tabs { display: flex; gap: 0; border-bottom: 1px solid ${COLORS.border}; margin-bottom: 24px; }
.tab { padding: 10px 20px; font-size: 13px; font-weight: 700; letter-spacing: 1px; cursor: pointer; color: ${COLORS.muted}; border-bottom: 2px solid transparent; transition: all 0.15s; }
.tab:hover { color: ${COLORS.text}; }
.tab.active { color: ${COLORS.text}; border-bottom-color: ${COLORS.ue5}; }
.tab.active.mc-tab { border-bottom-color: ${COLORS.mc}; }
.code-block { background: ${COLORS.surface2}; border: 1px solid ${COLORS.border}; border-radius: 6px; padding: 16px; font-family: 'JetBrains Mono', monospace; font-size: 12px; line-height: 1.7; color: #a0b0d0; overflow-x: auto; white-space: pre; }
.snippet-card { background: ${COLORS.surface}; border: 1px solid ${COLORS.border}; border-radius: 8px; padding: 16px; }
.snippet-title { font-size: 15px; font-weight: 700; letter-spacing: 1px; margin-bottom: 4px; }
.snippet-meta { display: flex; align-items: center; gap: 8px; margin-bottom: 12px; }
.checklist-item { display: flex; align-items: flex-start; gap: 10px; padding: 10px 0; border-bottom: 1px solid ${COLORS.border}; }
.checklist-item:last-child { border-bottom: none; }
.checkbox { width: 18px; height: 18px; border-radius: 3px; border: 2px solid ${COLORS.border}; background: transparent; cursor: pointer; flex-shrink: 0; display: flex; align-items: center; justify-content: center; transition: all 0.15s; margin-top: 1px; }
.checkbox.checked { background: ${COLORS.ue5}; border-color: ${COLORS.ue5}; }
.checkbox.checked.mc { background: ${COLORS.mc}; border-color: ${COLORS.mc}; }
.check-text { font-size: 14px; font-weight: 500; line-height: 1.4; }
.check-text.done { text-decoration: line-through; color: ${COLORS.muted}; }
.modal-bg { position: fixed; inset: 0; background: rgba(0,0,0,0.7); display: flex; align-items: center; justify-content: center; z-index: 100; backdrop-filter: blur(4px); }
.modal { background: ${COLORS.surface}; border: 1px solid ${COLORS.border}; border-radius: 10px; padding: 28px; width: 480px; max-width: 95vw; max-height: 90vh; overflow-y: auto; }
.modal-title { font-family: 'Bebas Neue', sans-serif; font-size: 24px; letter-spacing: 2px; margin-bottom: 20px; }
.modal-actions { display: flex; gap: 8px; justify-content: flex-end; margin-top: 20px; }
.empty-state { text-align: center; padding: 60px 20px; color: ${COLORS.muted}; }
.empty-icon { font-size: 48px; margin-bottom: 12px; opacity: 0.4; }
.empty-text { font-size: 15px; }
.stat-row { display: flex; justify-content: space-between; align-items: center; padding: 8px 0; border-bottom: 1px solid ${COLORS.border}; font-size: 14px; }
.stat-row:last-child { border-bottom: none; }
.top-bar { display: flex; justify-content: space-between; align-items: center; margin-bottom: 24px; }
.search-input { background: ${COLORS.surface}; border: 1px solid ${COLORS.border}; border-radius: 4px; padding: 8px 14px; color: ${COLORS.text}; font-family: 'Rajdhani', sans-serif; font-size: 14px; outline: none; width: 220px; }
.search-input:focus { border-color: ${COLORS.muted}; }
.copy-btn { position: absolute; top: 8px; right: 8px; }
.code-wrapper { position: relative; }
.tool-section { margin-bottom: 32px; }
.tool-section-title { font-size: 11px; font-weight: 700; letter-spacing: 2px; color: ${COLORS.muted}; margin-bottom: 16px; padding-bottom: 8px; border-bottom: 1px solid ${COLORS.border}; }
.progress-bar { height: 4px; background: ${COLORS.border}; border-radius: 2px; overflow: hidden; margin-top: 12px; }
.progress-fill { height: 100%; border-radius: 2px; transition: width 0.3s; }
.detail-header { display: flex; justify-content: space-between; align-items: flex-start; margin-bottom: 24px; }
.back-btn { display: flex; align-items: center; gap: 6px; color: ${COLORS.muted}; cursor: pointer; font-size: 13px; font-weight: 700; letter-spacing: 1px; margin-bottom: 20px; }
.back-btn:hover { color: ${COLORS.text}; }
.feature-tag { display: inline-flex; align-items: center; gap: 4px; padding: 3px 10px; background: ${COLORS.surface2}; border: 1px solid ${COLORS.border}; border-radius: 3px; font-size: 12px; font-weight: 600; margin: 3px; }
.feature-tag .del { cursor: pointer; color: ${COLORS.muted}; margin-left: 4px; }
.feature-tag .del:hover { color: ${COLORS.danger}; }
@media (max-width: 700px) { .sidebar { width: 60px; min-width: 60px; } .sidebar-logo { padding: 16px 10px; } .logo-text { font-size: 16px; } .logo-sub, .nav-item span, .sidebar-footer { display: none; } .nav-item { justify-content: center; padding: 12px; } .main { padding: 20px 16px; } .grid2, .grid3 { grid-template-columns: 1fr; } }
`;

const TEMPLATES = {
  mc_plugin: (name, pkg) => `// ${name}/src/main/java/${pkg.replace(/\./g, "/")}/${name}.java
package ${pkg};

import org.bukkit.plugin.java.JavaPlugin;

public final class ${name} extends JavaPlugin {

    @Override
    public void onEnable() {
        getLogger().info("${name} enabled!");
        // Register commands, listeners, etc.
    }

    @Override
    public void onDisable() {
        getLogger().info("${name} disabled!");
    }
}`,
  pom: (name, pkg) => `<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0
         http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>
    <groupId>${pkg}</groupId>
    <artifactId>${name.toLowerCase()}</artifactId>
    <version>1.0-SNAPSHOT</version>
    <packaging>jar</packaging>
    <repositories>
        <repository>
            <id>papermc</id>
            <url>https://repo.papermc.io/repository/maven-public/</url>
        </repository>
    </repositories>
    <dependencies>
        <dependency>
            <groupId>io.papermc.paper</groupId>
            <artifactId>paper-api</artifactId>
            <version>1.21.1-R0.1-SNAPSHOT</version>
            <scope>provided</scope>
        </dependency>
    </dependencies>
    <build>
        <plugins>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-shade-plugin</artifactId>
                <version>3.5.0</version>
            </plugin>
        </plugins>
    </build>
</project>`,
  ue5_actor: (name) => `// ${name}.h
#pragma once
#include "CoreMinimal.h"
#include "GameFramework/Actor.h"
#include "${name}.generated.h"

UCLASS()
class YOURPROJECT_API A${name} : public AActor {
    GENERATED_BODY()
public:
    A${name}();
    virtual void BeginPlay() override;
    virtual void Tick(float DeltaTime) override;

    UPROPERTY(EditAnywhere, BlueprintReadWrite, Category = "Config")
    float SomeValue = 1.0f;
};

// ${name}.cpp
#include "${name}.h"

A${name}::A${name}() {
    PrimaryActorTick.bCanEverTick = true;
}

void A${name}::BeginPlay() {
    Super::BeginPlay();
}

void A${name}::Tick(float DeltaTime) {
    Super::Tick(DeltaTime);
}`,
  ue5_component: (name) => `// ${name}Component.h
#pragma once
#include "CoreMinimal.h"
#include "Components/ActorComponent.h"
#include "${name}Component.generated.h"

UCLASS(ClassGroup=(Custom), meta=(BlueprintSpawnableComponent))
class YOURPROJECT_API U${name}Component : public UActorComponent {
    GENERATED_BODY()
public:
    U${name}Component();
    virtual void TickComponent(float DeltaTime, ELevelTick TickType,
        FActorComponentTickFunction* ThisTickFunction) override;
protected:
    virtual void BeginPlay() override;
};`,
};

const UE5_CHECKLIST = [
  { id: "ue1", text: "Project aangemaakt met C++ template", cat: "Setup" },
  { id: "ue2", text: "GameMode class geconfigureerd", cat: "Setup" },
  { id: "ue3", text: "PlayerController opgezet", cat: "Setup" },
  { id: "ue4", text: "Input mapping (Enhanced Input) geconfigureerd", cat: "Input" },
  { id: "ue5c", text: "Default pawn/character class ingesteld", cat: "Character" },
  { id: "ue6", text: "Collision presets gedefinieerd", cat: "Physics" },
  { id: "ue7", text: "Game instance voor persistent data", cat: "Data" },
  { id: "ue8", text: "Save game systeem opgezet", cat: "Data" },
  { id: "ue9", text: "HUD / UMG Widget opgezet", cat: "UI" },
  { id: "ue10", text: "Packaging instellingen gecheckt", cat: "Build" },
];

const MC_CHECKLIST = [
  { id: "mc1", text: "PaperMC jar gedownload (latest)", cat: "Setup" },
  { id: "mc2", text: "eula.txt geaccepteerd", cat: "Setup" },
  { id: "mc3", text: "server.properties geconfigureerd", cat: "Config" },
  { id: "mc4", text: "Maven project aangemaakt (plugin)", cat: "Plugin" },
  { id: "mc5", text: "plugin.yml ingevuld (name, version, main)", cat: "Plugin" },
  { id: "mc6", text: "JavaPlugin main class aangemaakt", cat: "Plugin" },
  { id: "mc7", text: "Commands geregistreerd in plugin.yml", cat: "Commands" },
  { id: "mc8", text: "EventListeners geregistreerd", cat: "Events" },
  { id: "mc9", text: "Resource pack aangemaken / gelinkt", cat: "Assets" },
  { id: "mc10", text: "Server getest in dev omgeving", cat: "Testing" },
];

// --- App ---
export default function DualCore() {
  const [page, setPage] = useState("dashboard");
  const [projects, setProjects] = useState([]);
  const [snippets, setSnippets] = useState([]);
  const [showAddProject, setShowAddProject] = useState(false);
  const [showAddSnippet, setShowAddSnippet] = useState(false);
  const [selectedProject, setSelectedProject] = useState(null);
  const [loaded, setLoaded] = useState(false);
  const [copied, setCopied] = useState(null);
  const [search, setSearch] = useState("");
  const [ue5Checks, setUe5Checks] = useState({});
  const [mcChecks, setMcChecks] = useState({});

  useEffect(() => {
    async function load() {
      try {
        const p = await window.storage.get("dc_projects");
        if (p) setProjects(JSON.parse(p.value));
      } catch {}
      try {
        const s = await window.storage.get("dc_snippets");
        if (s) setSnippets(JSON.parse(s.value));
      } catch {}
      try {
        const uc = await window.storage.get("dc_ue5checks");
        if (uc) setUe5Checks(JSON.parse(uc.value));
      } catch {}
      try {
        const mc = await window.storage.get("dc_mcchecks");
        if (mc) setMcChecks(JSON.parse(mc.value));
      } catch {}
      setLoaded(true);
    }
    load();
  }, []);

  const saveProjects = useCallback(async (arr) => {
    setProjects(arr);
    await window.storage.set("dc_projects", JSON.stringify(arr));
  }, []);

  const saveSnippets = useCallback(async (arr) => {
    setSnippets(arr);
    await window.storage.set("dc_snippets", JSON.stringify(arr));
  }, []);

  const copyText = (text, key) => {
    navigator.clipboard.writeText(text).then(() => {
      setCopied(key);
      setTimeout(() => setCopied(null), 1500);
    });
  };

  const ue5Count = projects.filter(p => p.type === "ue5").length;
  const mcCount = projects.filter(p => p.type === "mc").length;
  const activeCount = projects.filter(p => p.status === "active").length;

  if (!loaded) return (
    <div style={{ display: "flex", alignItems: "center", justifyContent: "center", height: "100vh", background: COLORS.bg, color: COLORS.muted, fontFamily: "Rajdhani", letterSpacing: 3, fontSize: 14 }}>
      LOADING DUALCORE...
    </div>
  );

  return (
    <>
      <style>{fonts}{css}</style>
      <div className="app">
        <Sidebar page={page} setPage={setPage} />
        <div className="main">
          {page === "dashboard" && <Dashboard projects={projects} ue5Count={ue5Count} mcCount={mcCount} activeCount={activeCount} snippets={snippets} setPage={setPage} />}
          {page === "projects" && <Projects projects={projects} saveProjects={saveProjects} showAdd={showAddProject} setShowAdd={setShowAddProject} search={search} setSearch={setSearch} selectedProject={selectedProject} setSelectedProject={setSelectedProject} />}
          {page === "tools" && <Tools copyText={copyText} copied={copied} />}
          {page === "snippets" && <Snippets snippets={snippets} saveSnippets={saveSnippets} showAdd={showAddSnippet} setShowAdd={setShowAddSnippet} copyText={copyText} copied={copied} />}
          {page === "checklist" && <Checklist ue5Checks={ue5Checks} setUe5Checks={setUe5Checks} mcChecks={mcChecks} setMcChecks={setMcChecks} />}
        </div>
      </div>
    </>
  );
}

function Sidebar({ page, setPage }) {
  const items = [
    { id: "dashboard", icon: "⬛", label: "DASHBOARD" },
    { id: "projects", icon: "📁", label: "PROJECTS" },
    { id: "tools", icon: "🔧", label: "TOOLS" },
    { id: "snippets", icon: "💾", label: "SNIPPETS" },
    { id: "checklist", icon: "☑️", label: "CHECKLIST" },
  ];
  return (
    <div className="sidebar">
      <div className="sidebar-logo">
        <div className="logo-text">DUALCORE</div>
        <div className="logo-sub">UE5 + MC SUITE</div>
      </div>
      <nav className="nav">
        {items.map(i => (
          <div key={i.id} className={`nav-item ${page === i.id ? "active" : ""}`} onClick={() => setPage(i.id)}>
            <span className="icon">{i.icon}</span>
            <span>{i.label}</span>
          </div>
        ))}
      </nav>
      <div className="sidebar-footer">
        <div className="version">v1.0.0</div>
      </div>
    </div>
  );
}

function Dashboard({ projects, ue5Count, mcCount, activeCount, snippets, setPage }) {
  const recent = [...projects].sort((a,b) => b.created - a.created).slice(0, 3);
  return (
    <div>
      <div className="page-header">
        <div className="page-title">DASHBOARD</div>
        <div className="page-sub">// all systems operational</div>
      </div>
      <div className="grid3" style={{ marginBottom: 24 }}>
        <div className="card">
          <div className="card-title">UE5 PROJECTS</div>
          <div className="card-value ue5-color">{ue5Count}</div>
        </div>
        <div className="card">
          <div className="card-title">MC PROJECTS</div>
          <div className="card-value mc-color">{mcCount}</div>
        </div>
        <div className="card">
          <div className="card-title">ACTIVE</div>
          <div className="card-value" style={{ color: COLORS.text }}>{activeCount}</div>
        </div>
      </div>
      <div className="grid2">
        <div className="card">
          <div className="card-title">RECENT PROJECTS</div>
          {recent.length === 0 ? <div style={{ color: COLORS.muted, fontSize: 13, marginTop: 8 }}>Geen projecten. Maak er een aan!</div> : recent.map(p => (
            <div key={p.id} className="stat-row" style={{ cursor: "pointer" }} onClick={() => setPage("projects")}>
              <span style={{ fontWeight: 600, fontSize: 14 }}>{p.name}</span>
              <span className={`badge badge-${p.type}`}>{p.type.toUpperCase()}</span>
            </div>
          ))}
          <div style={{ marginTop: 12 }}>
            <button className="btn btn-ghost btn-sm" onClick={() => setPage("projects")}>ALLE PROJECTEN →</button>
          </div>
        </div>
        <div className="card">
          <div className="card-title">QUICK STATS</div>
          <div className="stat-row"><span>Totale projecten</span><span style={{ fontWeight: 700 }}>{projects.length}</span></div>
          <div className="stat-row"><span>Snippets opgeslagen</span><span style={{ fontWeight: 700 }}>{snippets.length}</span></div>
          <div className="stat-row"><span>Gepauzeerd</span><span style={{ fontWeight: 700, color: COLORS.muted }}>{projects.filter(p => p.status === "paused").length}</span></div>
          <div className="stat-row"><span>Afgerond</span><span style={{ fontWeight: 700, color: COLORS.ue5 }}>{projects.filter(p => p.status === "done").length}</span></div>
          <div style={{ marginTop: 16 }}>
            <button className="btn btn-ghost btn-sm" onClick={() => setPage("tools")}>OPEN TOOLS →</button>
          </div>
        </div>
      </div>
    </div>
  );
}

function Projects({ projects, saveProjects, showAdd, setShowAdd, search, setSearch, selectedProject, setSelectedProject }) {
  const filtered = projects.filter(p => p.name.toLowerCase().includes(search.toLowerCase()));

  if (selectedProject) {
    return <ProjectDetail project={selectedProject} projects={projects} saveProjects={saveProjects} onBack={() => setSelectedProject(null)} />;
  }

  return (
    <div>
      <div className="top-bar">
        <div>
          <div className="page-title">PROJECTS</div>
          <div className="page-sub">// {projects.length} total</div>
        </div>
        <div style={{ display: "flex", gap: 8, alignItems: "center" }}>
          <input className="search-input" placeholder="Zoeken..." value={search} onChange={e => setSearch(e.target.value)} />
          <button className="btn btn-primary" onClick={() => setShowAdd(true)}>+ NIEUW</button>
        </div>
      </div>
      {filtered.length === 0 ? (
        <div className="empty-state">
          <div className="empty-icon">📁</div>
          <div className="empty-text">Nog geen projecten. Maak er een aan!</div>
        </div>
      ) : (
        <div className="grid2">
          {filtered.map(p => (
            <div key={p.id} className={`project-card ${p.type}`} onClick={() => setSelectedProject(p)}>
              <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start" }}>
                <span className={`badge badge-${p.type}`}>{p.type === "ue5" ? "UNREAL ENGINE 5" : "MINECRAFT"}</span>
                <span className={`badge badge-${p.status}`}>{p.status.toUpperCase()}</span>
              </div>
              <div className="project-name">{p.name}</div>
              <div className="project-desc">{p.description || "Geen omschrijving."}</div>
              <div className="project-meta">
                {(p.features || []).slice(0, 3).map((f, i) => (
                  <span key={i} className="feature-tag">{f}</span>
                ))}
                {(p.features || []).length > 3 && <span style={{ fontSize: 12, color: COLORS.muted }}>+{p.features.length - 3} meer</span>}
              </div>
              <div className="progress-bar" style={{ marginTop: 14 }}>
                <div className="progress-fill" style={{ width: `${p.progress || 0}%`, background: p.type === "ue5" ? COLORS.ue5 : COLORS.mc }} />
              </div>
              <div style={{ fontSize: 11, color: COLORS.muted, marginTop: 4, fontFamily: "JetBrains Mono, monospace" }}>{p.progress || 0}% voltooid</div>
            </div>
          ))}
        </div>
      )}
      {showAdd && <AddProjectModal onClose={() => setShowAdd(false)} onAdd={async (proj) => {
        const updated = [...projects, proj];
        await saveProjects(updated);
        setShowAdd(false);
      }} />}
    </div>
  );
}

function ProjectDetail({ project, projects, saveProjects, onBack }) {
  const [proj, setProj] = useState({ ...project });
  const [newFeature, setNewFeature] = useState("");
  const [newNote, setNewNote] = useState(proj.notes || "");

  const save = async (updated) => {
    const arr = projects.map(p => p.id === updated.id ? updated : p);
    await saveProjects(arr);
    setProj(updated);
  };

  const addFeature = async () => {
    if (!newFeature.trim()) return;
    const updated = { ...proj, features: [...(proj.features || []), newFeature.trim()] };
    await save(updated);
    setNewFeature("");
  };

  const removeFeature = async (f) => {
    const updated = { ...proj, features: proj.features.filter(x => x !== f) };
    await save(updated);
  };

  const setProgress = async (val) => {
    const updated = { ...proj, progress: Number(val) };
    await save(updated);
  };

  const setStatus = async (val) => {
    const updated = { ...proj, status: val };
    await save(updated);
  };

  const saveNotes = async () => {
    const updated = { ...proj, notes: newNote };
    await save(updated);
  };

  const deleteProject = async () => {
    const arr = projects.filter(p => p.id !== proj.id);
    await saveProjects(arr);
    onBack();
  };

  return (
    <div>
      <div className="back-btn" onClick={onBack}>← TERUG</div>
      <div className="detail-header">
        <div>
          <div style={{ display: "flex", gap: 8, marginBottom: 8 }}>
            <span className={`badge badge-${proj.type}`}>{proj.type === "ue5" ? "UNREAL ENGINE 5" : "MINECRAFT"}</span>
            <span className={`badge badge-${proj.status}`}>{proj.status.toUpperCase()}</span>
          </div>
          <div style={{ fontSize: 32, fontFamily: "Bebas Neue", letterSpacing: 2 }}>{proj.name}</div>
          <div style={{ color: COLORS.muted, fontSize: 13, marginTop: 4 }}>{proj.description}</div>
        </div>
        <button className="btn btn-danger btn-sm" onClick={deleteProject}>VERWIJDER</button>
      </div>
      <div className="grid2">
        <div>
          <div className="card" style={{ marginBottom: 16 }}>
            <div className="card-title">VOORTGANG</div>
            <input type="range" min="0" max="100" value={proj.progress || 0} onChange={e => setProgress(e.target.value)} style={{ width: "100%", accentColor: proj.type === "ue5" ? COLORS.ue5 : COLORS.mc, margin: "8px 0" }} />
            <div style={{ fontFamily: "Bebas Neue", fontSize: 32, letterSpacing: 2, color: proj.type === "ue5" ? COLORS.ue5 : COLORS.mc }}>{proj.progress || 0}%</div>
          </div>
          <div className="card">
            <div className="card-title">STATUS</div>
            <select className="input select" value={proj.status} onChange={e => setStatus(e.target.value)} style={{ marginTop: 8 }}>
              <option value="active">Active</option>
              <option value="paused">Paused</option>
              <option value="done">Done</option>
            </select>
          </div>
        </div>
        <div>
          <div className="card">
            <div className="card-title">FEATURES</div>
            <div style={{ display: "flex", flexWrap: "wrap", marginBottom: 12, marginTop: 8 }}>
              {(proj.features || []).map((f, i) => (
                <span key={i} className="feature-tag">{f}<span className="del" onClick={() => removeFeature(f)}>×</span></span>
              ))}
            </div>
            <div style={{ display: "flex", gap: 8 }}>
              <input className="input" placeholder="Nieuwe feature..." value={newFeature} onChange={e => setNewFeature(e.target.value)} onKeyDown={e => e.key === "Enter" && addFeature()} style={{ fontSize: 13 }} />
              <button className="btn btn-primary btn-sm" onClick={addFeature}>+</button>
            </div>
          </div>
        </div>
      </div>
      <div className="card" style={{ marginTop: 16 }}>
        <div className="card-title">NOTITIES</div>
        <textarea className="input textarea" value={newNote} onChange={e => setNewNote(e.target.value)} placeholder="Aantekeningen, ideeën, bugs..." style={{ marginTop: 8 }} />
        <button className="btn btn-ghost btn-sm" style={{ marginTop: 8 }} onClick={saveNotes}>OPSLAAN</button>
      </div>
    </div>
  );
}

function AddProjectModal({ onClose, onAdd }) {
  const [form, setForm] = useState({ name: "", type: "mc", description: "", status: "active", progress: 0, features: [], notes: "" });
  const set = (k, v) => setForm(f => ({ ...f, [k]: v }));

  return (
    <div className="modal-bg" onClick={onClose}>
      <div className="modal" onClick={e => e.stopPropagation()}>
        <div className="modal-title">NIEUW PROJECT</div>
        <div className="form-group">
          <label className="label">NAAM</label>
          <input className="input" placeholder="EclipseSMP, StitchBorn..." value={form.name} onChange={e => set("name", e.target.value)} />
        </div>
        <div className="form-group">
          <label className="label">TYPE</label>
          <select className="input select" value={form.type} onChange={e => set("type", e.target.value)}>
            <option value="mc">Minecraft Server</option>
            <option value="ue5">Unreal Engine 5</option>
          </select>
        </div>
        <div className="form-group">
          <label className="label">OMSCHRIJVING</label>
          <textarea className="input textarea" placeholder="Kort omschrijven..." value={form.description} onChange={e => set("description", e.target.value)} />
        </div>
        <div className="form-group">
          <label className="label">STATUS</label>
          <select className="input select" value={form.status} onChange={e => set("status", e.target.value)}>
            <option value="active">Active</option>
            <option value="paused">Paused</option>
            <option value="done">Done</option>
          </select>
        </div>
        <div className="modal-actions">
          <button className="btn btn-ghost" onClick={onClose}>ANNULEER</button>
          <button className="btn btn-primary" onClick={() => {
            if (!form.name.trim()) return;
            onAdd({ ...form, id: Date.now(), created: Date.now() });
          }}>AANMAKEN</button>
        </div>
      </div>
    </div>
  );
}

function Tools({ copyText, copied }) {
  const [tab, setTab] = useState("mc");
  const [mcPlugin, setMcPlugin] = useState({ name: "MyPlugin", pkg: "nl.myserver.myplugin" });
  const [ue5Actor, setUe5Actor] = useState({ name: "MyActor", type: "actor" });
  const [props, setProps] = useState({
    server_port: "25565", max_players: "20", gamemode: "survival",
    difficulty: "normal", pvp: "true", online_mode: "true",
    motd: "A Minecraft Server", level_name: "world",
    view_distance: "10", spawn_protection: "16"
  });

  const serverProps = Object.entries(props).map(([k, v]) => `${k}=${v}`).join("\n");
  const pluginCode = TEMPLATES.mc_plugin(mcPlugin.name, mcPlugin.pkg);
  const pomCode = TEMPLATES.pom(mcPlugin.name, mcPlugin.pkg);
  const ue5Code = ue5Actor.type === "actor" ? TEMPLATES.ue5_actor(ue5Actor.name) : TEMPLATES.ue5_component(ue5Actor.name);

  return (
    <div>
      <div className="page-header">
        <div className="page-title">TOOLS</div>
        <div className="page-sub">// generators & templates</div>
      </div>
      <div className="tabs">
        <div className={`tab mc-tab ${tab === "mc" ? "active" : ""}`} onClick={() => setTab("mc")}>⛏ MINECRAFT</div>
        <div className={`tab ${tab === "ue5" ? "active" : ""}`} onClick={() => setTab("ue5")}>🎮 UNREAL ENGINE 5</div>
      </div>

      {tab === "mc" && (
        <div>
          <div className="tool-section">
            <div className="tool-section-title">SERVER.PROPERTIES GENERATOR</div>
            <div className="grid2" style={{ marginBottom: 16 }}>
              {Object.entries(props).map(([k, v]) => (
                <div key={k} className="form-group" style={{ marginBottom: 10 }}>
                  <label className="label">{k.replace(/_/g, " ").toUpperCase()}</label>
                  <input className="input" value={v} onChange={e => setProps(p => ({ ...p, [k]: e.target.value }))} />
                </div>
              ))}
            </div>
            <div className="code-wrapper">
              <div className="code-block">{serverProps}</div>
              <button className="btn btn-mc btn-sm copy-btn" onClick={() => copyText(serverProps, "props")}>{copied === "props" ? "✓ COPIED" : "COPY"}</button>
            </div>
          </div>

          <div className="tool-section">
            <div className="tool-section-title">PAPERMC PLUGIN BOILERPLATE</div>
            <div className="grid2" style={{ marginBottom: 16 }}>
              <div className="form-group">
                <label className="label">PLUGIN NAAM</label>
                <input className="input" value={mcPlugin.name} onChange={e => setMcPlugin(p => ({ ...p, name: e.target.value }))} />
              </div>
              <div className="form-group">
                <label className="label">PACKAGE</label>
                <input className="input" value={mcPlugin.pkg} onChange={e => setMcPlugin(p => ({ ...p, pkg: e.target.value }))} />
              </div>
            </div>
            <div style={{ marginBottom: 12 }}>
              <div style={{ fontSize: 11, color: COLORS.muted, marginBottom: 6, fontFamily: "JetBrains Mono", letterSpacing: 1 }}>MAIN CLASS</div>
              <div className="code-wrapper">
                <div className="code-block">{pluginCode}</div>
                <button className="btn btn-mc btn-sm copy-btn" onClick={() => copyText(pluginCode, "plugin")}>{copied === "plugin" ? "✓ COPIED" : "COPY"}</button>
              </div>
            </div>
            <div>
              <div style={{ fontSize: 11, color: COLORS.muted, marginBottom: 6, fontFamily: "JetBrains Mono", letterSpacing: 1 }}>POM.XML</div>
              <div className="code-wrapper">
                <div className="code-block">{pomCode}</div>
                <button className="btn btn-mc btn-sm copy-btn" onClick={() => copyText(pomCode, "pom")}>{copied === "pom" ? "✓ COPIED" : "COPY"}</button>
              </div>
            </div>
          </div>
        </div>
      )}

      {tab === "ue5" && (
        <div>
          <div className="tool-section">
            <div className="tool-section-title">C++ CLASS GENERATOR</div>
            <div className="grid2" style={{ marginBottom: 16 }}>
              <div className="form-group">
                <label className="label">KLASSE NAAM</label>
                <input className="input" value={ue5Actor.name} onChange={e => setUe5Actor(p => ({ ...p, name: e.target.value }))} />
              </div>
              <div className="form-group">
                <label className="label">TYPE</label>
                <select className="input select" value={ue5Actor.type} onChange={e => setUe5Actor(p => ({ ...p, type: e.target.value }))}>
                  <option value="actor">Actor (AActor)</option>
                  <option value="component">ActorComponent</option>
                </select>
              </div>
            </div>
            <div className="code-wrapper">
              <div className="code-block">{ue5Code}</div>
              <button className="btn btn-primary btn-sm copy-btn" onClick={() => copyText(ue5Code, "ue5")}>{copied === "ue5" ? "✓ COPIED" : "COPY"}</button>
            </div>
          </div>
        </div>
      )}
    </div>
  );
}

function Snippets({ snippets, saveSnippets, showAdd, setShowAdd, copyText, copied }) {
  const [filterType, setFilterType] = useState("all");
  const filtered = snippets.filter(s => filterType === "all" || s.type === filterType);

  return (
    <div>
      <div className="top-bar">
        <div>
          <div className="page-title">SNIPPETS</div>
          <div className="page-sub">// {snippets.length} opgeslagen</div>
        </div>
        <div style={{ display: "flex", gap: 8 }}>
          <select className="input select" style={{ width: 140 }} value={filterType} onChange={e => setFilterType(e.target.value)}>
            <option value="all">Alle</option>
            <option value="mc">Minecraft</option>
            <option value="ue5">UE5</option>
            <option value="other">Overig</option>
          </select>
          <button className="btn btn-primary" onClick={() => setShowAdd(true)}>+ NIEUW</button>
        </div>
      </div>
      {filtered.length === 0 ? (
        <div className="empty-state">
          <div className="empty-icon">💾</div>
          <div className="empty-text">Geen snippets gevonden.</div>
        </div>
      ) : (
        <div style={{ display: "flex", flexDirection: "column", gap: 12 }}>
          {filtered.map(s => (
            <div key={s.id} className="snippet-card">
              <div className="snippet-title">{s.title}</div>
              <div className="snippet-meta">
                <span className={`badge badge-${s.type}`}>{s.type.toUpperCase()}</span>
                {s.lang && <span style={{ fontSize: 11, color: COLORS.muted, fontFamily: "JetBrains Mono" }}>{s.lang}</span>}
              </div>
              <div className="code-wrapper">
                <div className="code-block" style={{ maxHeight: 200, overflow: "auto" }}>{s.code}</div>
                <div style={{ display: "flex", gap: 6, marginTop: 8, justifyContent: "flex-end" }}>
                  <button className="btn btn-ghost btn-sm" onClick={() => copyText(s.code, `snip_${s.id}`)}>{copied === `snip_${s.id}` ? "✓ COPIED" : "COPY"}</button>
                  <button className="btn btn-danger btn-sm" onClick={async () => {
                    const updated = snippets.filter(x => x.id !== s.id);
                    await saveSnippets(updated);
                  }}>DEL</button>
                </div>
              </div>
            </div>
          ))}
        </div>
      )}
      {showAdd && <AddSnippetModal onClose={() => setShowAdd(false)} onAdd={async (s) => {
        const updated = [...snippets, s];
        await saveSnippets(updated);
        setShowAdd(false);
      }} />}
    </div>
  );
}

function AddSnippetModal({ onClose, onAdd }) {
  const [form, setForm] = useState({ title: "", type: "mc", lang: "java", code: "" });
  const set = (k, v) => setForm(f => ({ ...f, [k]: v }));
  return (
    <div className="modal-bg" onClick={onClose}>
      <div className="modal" onClick={e => e.stopPropagation()}>
        <div className="modal-title">SNIPPET OPSLAAN</div>
        <div className="form-group">
          <label className="label">TITEL</label>
          <input className="input" placeholder="Naam van snippet..." value={form.title} onChange={e => set("title", e.target.value)} />
        </div>
        <div className="grid2">
          <div className="form-group">
            <label className="label">TYPE</label>
            <select className="input select" value={form.type} onChange={e => set("type", e.target.value)}>
              <option value="mc">Minecraft</option>
              <option value="ue5">UE5</option>
              <option value="other">Overig</option>
            </select>
          </div>
          <div className="form-group">
            <label className="label">TAAL</label>
            <input className="input" placeholder="java, cpp, kotlin..." value={form.lang} onChange={e => set("lang", e.target.value)} />
          </div>
        </div>
        <div className="form-group">
          <label className="label">CODE</label>
          <textarea className="input textarea" style={{ minHeight: 140, fontFamily: "JetBrains Mono, monospace", fontSize: 12 }} placeholder="Plak je code hier..." value={form.code} onChange={e => set("code", e.target.value)} />
        </div>
        <div className="modal-actions">
          <button className="btn btn-ghost" onClick={onClose}>ANNULEER</button>
          <button className="btn btn-primary" onClick={() => {
            if (!form.title.trim() || !form.code.trim()) return;
            onAdd({ ...form, id: Date.now() });
          }}>OPSLAAN</button>
        </div>
      </div>
    </div>
  );
}

function Checklist({ ue5Checks, setUe5Checks, mcChecks, setMcChecks }) {
  const [tab, setTab] = useState("ue5");

  const toggleUE5 = async (id) => {
    const updated = { ...ue5Checks, [id]: !ue5Checks[id] };
    setUe5Checks(updated);
    await window.storage.set("dc_ue5checks", JSON.stringify(updated));
  };

  const toggleMC = async (id) => {
    const updated = { ...mcChecks, [id]: !mcChecks[id] };
    setMcChecks(updated);
    await window.storage.set("dc_mcchecks", JSON.stringify(updated));
  };

  const ue5Done = UE5_CHECKLIST.filter(i => ue5Checks[i.id]).length;
  const mcDone = MC_CHECKLIST.filter(i => mcChecks[i.id]).length;

  return (
    <div>
      <div className="page-header">
        <div className="page-title">SETUP CHECKLIST</div>
        <div className="page-sub">// project setup guides</div>
      </div>
      <div className="tabs">
        <div className={`tab ${tab === "ue5" ? "active" : ""}`} onClick={() => setTab("ue5")}>🎮 UE5 — {ue5Done}/{UE5_CHECKLIST.length}</div>
        <div className={`tab mc-tab ${tab === "mc" ? "active" : ""}`} onClick={() => setTab("mc")}>⛏ MINECRAFT — {mcDone}/{MC_CHECKLIST.length}</div>
      </div>
      <div className="card">
        <div className="progress-bar" style={{ marginBottom: 20 }}>
          <div className="progress-fill" style={{
            width: tab === "ue5" ? `${(ue5Done / UE5_CHECKLIST.length) * 100}%` : `${(mcDone / MC_CHECKLIST.length) * 100}%`,
            background: tab === "ue5" ? COLORS.ue5 : COLORS.mc
          }} />
        </div>
        {(tab === "ue5" ? UE5_CHECKLIST : MC_CHECKLIST).map(item => {
          const checked = tab === "ue5" ? !!ue5Checks[item.id] : !!mcChecks[item.id];
          return (
            <div key={item.id} className="checklist-item">
              <div className={`checkbox ${checked ? "checked" : ""} ${tab === "mc" ? "mc" : ""}`} onClick={() => tab === "ue5" ? toggleUE5(item.id) : toggleMC(item.id)}>
                {checked && <span style={{ fontSize: 10, color: "#07070f", fontWeight: 900 }}>✓</span>}
              </div>
              <div>
                <div className={`check-text ${checked ? "done" : ""}`}>{item.text}</div>
                <div style={{ fontSize: 11, color: COLORS.muted, fontFamily: "JetBrains Mono", marginTop: 2 }}>{item.cat}</div>
              </div>
            </div>
          );
        })}
      </div>
    </div>
  );
}
