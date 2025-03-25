# Os-project-
Deadlock detection 
# ====================== Module 3: Main ======================
if __name__ == "__main__":
    root = Tk()
    app = ResourceAllocationGraphSimulator(root)
    root.mainloop()
    def analyze_graph(self):
        """
        Analyzes the graph for deadlocks and visualizes it.
        """
        if not self.graph.edges:
            messagebox.showerror("Error", "No edges added to the graph.")
            return
