# homework

PluginDescriptionFile pdffile =  getDescription();
	public String version = pdffile.getVersion();
	public String name = pdffile.getName();
	@Override
    public void onEnable() {
		Bukkit.getConsoleSender()
		.sendMessage
		("El plugin: " + name + " ha sido activado (version:" + version + ")"  );
		Bukkit.getPluginManager().registerEvents(new Join(this),this);
    }
    
    @Override
    public void onDisable() {

    }
