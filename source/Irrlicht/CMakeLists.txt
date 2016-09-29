set (IRRMESHLOADER CBSPMeshFileLoader.cpp CMD2MeshFileLoader.cpp CMD3MeshFileLoader.cpp CMS3DMeshFileLoader.cpp CB3DMeshFileLoader.cpp C3DSMeshFileLoader.cpp COgreMeshFileLoader.cpp COBJMeshFileLoader.cpp CColladaFileLoader.cpp CCSMLoader.cpp CDMFLoader.cpp CLMTSMeshFileLoader.cpp CMY3DMeshFileLoader.cpp COCTLoader.cpp CXMeshFileLoader.cpp CIrrMeshFileLoader.cpp CSTLMeshFileLoader.cpp CLWOMeshFileLoader.cpp CPLYMeshFileLoader.cpp CSMFMeshFileLoader.cpp)

set (IRRMESHWRITER CColladaMeshWriter.cpp CIrrMeshWriter.cpp CSTLMeshWriter.cpp COBJMeshWriter.cpp CPLYMeshWriter.cpp)

set (IRRMESHOBJ ${IRRMESHLOADER} ${IRRMESHWRITER} CSkinnedMesh.cpp CBoneSceneNode.cpp CMeshSceneNode.cpp CAnimatedMeshSceneNode.cpp CAnimatedMeshMD2.cpp CAnimatedMeshMD3.cpp CQ3LevelMesh.cpp CQuake3ShaderSceneNode.cpp CAnimatedMeshHalfLife.cpp)

set (IRROBJ CBillboardSceneNode.cpp CCameraSceneNode.cpp CDummyTransformationSceneNode.cpp CEmptySceneNode.cpp CGeometryCreator.cpp CLightSceneNode.cpp CMeshManipulator.cpp CMetaTriangleSelector.cpp COctreeSceneNode.cpp COctreeTriangleSelector.cpp CSceneCollisionManager.cpp CSceneManager.cpp CShadowVolumeSceneNode.cpp CSkyBoxSceneNode.cpp CSkyDomeSceneNode.cpp CTerrainSceneNode.cpp CTerrainTriangleSelector.cpp CVolumeLightSceneNode.cpp CCubeSceneNode.cpp CSphereSceneNode.cpp CTextSceneNode.cpp CTriangleBBSelector.cpp CTriangleSelector.cpp CWaterSurfaceSceneNode.cpp CMeshCache.cpp CDefaultSceneNodeAnimatorFactory.cpp CDefaultSceneNodeFactory.cpp CSceneLoaderIrr.cpp)

set (IRRPARTICLEOBJ CParticleAnimatedMeshSceneNodeEmitter.cpp CParticleBoxEmitter.cpp CParticleCylinderEmitter.cpp CParticleMeshEmitter.cpp CParticlePointEmitter.cpp CParticleRingEmitter.cpp CParticleSphereEmitter.cpp CParticleAttractionAffector.cpp CParticleFadeOutAffector.cpp CParticleGravityAffector.cpp CParticleRotationAffector.cpp CParticleSystemSceneNode.cpp CParticleScaleAffector.cpp)

set (IRRANIMOBJ CSceneNodeAnimatorCameraFPS.cpp CSceneNodeAnimatorCameraMaya.cpp CSceneNodeAnimatorCollisionResponse.cpp CSceneNodeAnimatorDelete.cpp CSceneNodeAnimatorFlyCircle.cpp CSceneNodeAnimatorFlyStraight.cpp CSceneNodeAnimatorFollowSpline.cpp CSceneNodeAnimatorRotation.cpp CSceneNodeAnimatorTexture.cpp)

set (IRRDRVROBJ CNullDriver.cpp COpenGLDriver.cpp COpenGLNormalMapRenderer.cpp COpenGLParallaxMapRenderer.cpp COpenGLShaderMaterialRenderer.cpp COpenGLTexture.cpp COpenGLSLMaterialRenderer.cpp COpenGLExtensionHandler.cpp CD3D8Driver.cpp CD3D8NormalMapRenderer.cpp CD3D8ParallaxMapRenderer.cpp CD3D8ShaderMaterialRenderer.cpp CD3D8Texture.cpp CD3D9Driver.cpp CD3D9HLSLMaterialRenderer.cpp CD3D9NormalMapRenderer.cpp CD3D9ParallaxMapRenderer.cpp CD3D9ShaderMaterialRenderer.cpp CD3D9Texture.cpp)

set (IRRIMAGEOBJ CColorConverter.cpp CImage.cpp CImageLoaderBMP.cpp CImageLoaderDDS.cpp CImageLoaderJPG.cpp CImageLoaderPCX.cpp CImageLoaderPNG.cpp CImageLoaderPSD.cpp CImageLoaderTGA.cpp CImageLoaderPPM.cpp CImageLoaderWAL.cpp CImageLoaderRGB.cpp CImageWriterBMP.cpp CImageWriterJPG.cpp CImageWriterPCX.cpp CImageWriterPNG.cpp CImageWriterPPM.cpp CImageWriterPSD.cpp CImageWriterTGA.cpp)

set (IRRVIDEOOBJ CVideoModeList.cpp CFPSCounter.cpp ${IRRDRVROBJ} ${IRRIMAGEOBJ})

set (IRRSWRENDEROBJ CSoftwareDriver.cpp CSoftwareTexture.cpp CTRFlat.cpp CTRFlatWire.cpp CTRGouraud.cpp CTRGouraudWire.cpp CTRNormalMap.cpp CTRStencilShadow.cpp CTRTextureFlat.cpp CTRTextureFlatWire.cpp CTRTextureGouraud.cpp CTRTextureGouraudAdd.cpp CTRTextureGouraudNoZ.cpp CTRTextureGouraudWire.cpp CZBuffer.cpp CTRTextureGouraudVertexAlpha2.cpp CTRTextureGouraudNoZ2.cpp CTRTextureLightMap2_M2.cpp CTRTextureLightMap2_M4.cpp CTRTextureLightMap2_M1.cpp CSoftwareDriver2.cpp CSoftwareTexture2.cpp CTRTextureGouraud2.cpp CTRGouraud2.cpp CTRGouraudAlpha2.cpp CTRGouraudAlphaNoZ2.cpp CTRTextureDetailMap2.cpp CTRTextureGouraudAdd2.cpp CTRTextureGouraudAddNoZ2.cpp CTRTextureWire2.cpp CTRTextureLightMap2_Add.cpp CTRTextureLightMapGouraud2_M4.cpp IBurningShader.cpp CTRTextureBlend.cpp CTRTextureGouraudAlpha.cpp CTRTextureGouraudAlphaNoZ.cpp CDepthBuffer.cpp CBurningShader_Raster_Reference.cpp)

set (IRRIOOBJ CFileList.cpp CFileSystem.cpp CLimitReadFile.cpp CMemoryFile.cpp CReadFile.cpp CWriteFile.cpp CXMLReader.cpp CXMLWriter.cpp CWADReader.cpp CZipReader.cpp CPakReader.cpp CNPKReader.cpp CTarReader.cpp CMountPointReader.cpp irrXML.cpp CAttributes.cpp lzma/LzmaDec.c)

set (IRROTHEROBJ CIrrDeviceSDL.cpp CIrrDeviceLinux.cpp CIrrDeviceConsole.cpp CIrrDeviceStub.cpp CIrrDeviceWin32.cpp CIrrDeviceFB.cpp CLogger.cpp COSOperator.cpp Irrlicht.cpp os.cpp)

set (IRRGUIOBJ CGUIButton.cpp CGUICheckBox.cpp CGUIComboBox.cpp CGUIContextMenu.cpp CGUIEditBox.cpp CGUIEnvironment.cpp CGUIFileOpenDialog.cpp CGUIFont.cpp CGUIImage.cpp CGUIInOutFader.cpp CGUIListBox.cpp CGUIMenu.cpp CGUIMeshViewer.cpp CGUIMessageBox.cpp CGUIModalScreen.cpp CGUIScrollBar.cpp CGUISpinBox.cpp CGUISkin.cpp CGUIStaticText.cpp CGUITabControl.cpp CGUITable.cpp CGUIToolBar.cpp CGUIWindow.cpp CGUIColorSelectDialog.cpp CDefaultGUIElementFactory.cpp CGUISpriteBank.cpp CGUIImageList.cpp CGUITreeView.cpp)

set (ZLIBOBJ zlib/adler32.c zlib/compress.c zlib/crc32.c zlib/deflate.c zlib/inffast.c zlib/inflate.c zlib/inftrees.c zlib/trees.c zlib/uncompr.c zlib/zutil.c)

set (JPEGLIBOBJ jpeglib/jcapimin.c jpeglib/jcapistd.c jpeglib/jccoefct.c jpeglib/jccolor.c jpeglib/jcdctmgr.c jpeglib/jchuff.c jpeglib/jcinit.c jpeglib/jcmainct.c jpeglib/jcmarker.c jpeglib/jcmaster.c jpeglib/jcomapi.c jpeglib/jcparam.c jpeglib/jcprepct.c jpeglib/jcsample.c jpeglib/jctrans.c jpeglib/jdapimin.c jpeglib/jdapistd.c jpeglib/jdatadst.c jpeglib/jdatasrc.c jpeglib/jdcoefct.c jpeglib/jdcolor.c jpeglib/jddctmgr.c jpeglib/jdhuff.c jpeglib/jdinput.c jpeglib/jdmainct.c jpeglib/jdmarker.c jpeglib/jdmaster.c jpeglib/jdmerge.c jpeglib/jdpostct.c jpeglib/jdsample.c jpeglib/jdtrans.c jpeglib/jerror.c jpeglib/jfdctflt.c jpeglib/jfdctfst.c jpeglib/jfdctint.c jpeglib/jidctflt.c jpeglib/jidctfst.c jpeglib/jidctint.c jpeglib/jmemmgr.c jpeglib/jmemnobs.c jpeglib/jquant1.c jpeglib/jquant2.c jpeglib/jutils.c jpeglib/jcarith.c jpeglib/jdarith.c jpeglib/jaricom.c)

set (LIBPNGOBJ libpng/png.c libpng/pngerror.c libpng/pngget.c libpng/pngmem.c libpng/pngpread.c libpng/pngread.c libpng/pngrio.c libpng/pngrtran.c libpng/pngrutil.c libpng/pngset.c libpng/pngtrans.c libpng/pngwio.c libpng/pngwrite.c libpng/pngwtran.c libpng/pngwutil.c)

set (LIBAESGM aesGladman/aescrypt.cpp aesGladman/aeskey.cpp aesGladman/aestab.cpp aesGladman/fileenc.cpp aesGladman/hmac.cpp aesGladman/prng.cpp aesGladman/pwd2key.cpp aesGladman/sha1.cpp aesGladman/sha2.cpp)

set (BZIP2OBJ bzip2/blocksort.c bzip2/huffman.c bzip2/crctable.c bzip2/randtable.c bzip2/bzcompress.c bzip2/decompress.c bzip2/bzlib.c)

set (EXTRAOBJ )

set (LINKOBJ ${IRRMESHOBJ} ${IRROBJ} ${IRRPARTICLEOBJ} ${IRRANIMOBJ} ${IRRVIDEOOBJ} ${IRRSWRENDEROBJ} ${IRRIOOBJ} ${IRROTHEROBJ} ${IRRGUIOBJ} ${ZLIBOBJ} ${JPEGLIBOBJ} ${LIBPNGOBJ} ${LIBAESGM} ${BZIP2OBJ} ${EXTRAOBJ})

# Linux specific options
if (${CMAKE_SYSTEM_NAME} MATCHES "Linux")
  link_directories (/usr/X11R6/lib)

# OSX specific options
elseif (${CMAKE_SYSTEM_NAME} MATCHES "Darwin")
  set (IRROTHEROBJ
    ${IRROTHEROBJ}
    MacOSX/CIrrDeviceMacOSX.cpp
    MacOSX/OSXClipboard.cpp
    MacOSX/AppDelegate.cpp
  )
  link_directories (/usr/X11R6/lib)
  set (CMAKE_EXE_LINKER_FLAGS "--no-export-all-symbols --add-stdcall-alias" CACHE STRING "Flags used by the linker." FORCE)

# Windows specific options
elseif (WIN32)
  set (CMAKE_EXE_LINKER_FLAGS "-Wl,--add-stdcall-alias" CACHE STRING "Flags used by the linker." FORCE)
endif (${CMAKE_SYSTEM_NAME} MATCHES "Linux")

# Add the library
set (LIBRARY_BUILD_TYPE STATIC)
if (BUILD_SHARED_LIBS)
  set (LIBRARY_BUILD_TYPE SHARED)
endif (BUILD_SHARED_LIBS)
add_library (${PROJECT_NAME} ${LIBRARY_BUILD_TYPE} ${LINKOBJ})

# Linux specific options
if (${CMAKE_SYSTEM_NAME} MATCHES "Linux")
  target_link_libraries (${PROJECT_NAME} GL Xxf86vm)
  
# OSX specific options
elseif (${CMAKE_SYSTEM_NAME} MATCHES "Darwin")
  target_link_libraries (${PROJECT_NAME} GL Xxf86vm)

# Windows specific options
elseif (WIN32)
  target_link_libraries (${PROJECT_NAME} gdi32 opengl32 d3dx9d winmm)
endif (${CMAKE_SYSTEM_NAME} MATCHES "Linux")

set (ENABLE_CPP11 0 CACHE BOOL "Compile with C++11")

if (ENABLE_CPP11)
  set_property(TARGET ${PROJECT_NAME} PROPERTY CXX_STANDARD 11)
endif (ENABLE_CPP11)